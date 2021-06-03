Exercise 3.5

@Test
public void testSort()
{

	names.add("Laura");
	names.add("Han");
	names.add("Alex");
	names.add("Ashley");
	names.sort();
	asserTrue("Sort method", names.getFirst().equals("Alex"));
}


This assertion only check for the first element.

RIRP model:
- Reachability: In case there's a fault with the first element at that point it is reached. For the first element, it isn't come to
- Infection: Yes.
- Propagation: No. The full list can be sorted erroneously but the primary component can still be "Alex". The test condition would still be satified and return redress whereas the tainted state is still not dectected.
- Revealability: No. The test declaration cannot uncover the fault.