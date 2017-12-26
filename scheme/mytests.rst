This file holds the tests that you create. Remember to import the python file(s)
you wish to test, along with any other modules you may need.
Run your tests with "python3 ok -t --suite SUITE_NAME --case CASE_NAME -v"
--------------------------------------------------------------------------------

Suite 5

	>>> from scheme import *
    >>> from scheme_reader import *

    Case 1
    	>>> expr = read_line('(- (+ 2 2) 1)')
    	>>> scheme_eval(expr, create_global_frame())
    	3

Suite 8
	
	>>> from scheme import *
    >>> from scheme_reader import *

    Case 1
    	>>> eval_all(Pair(nil, Pair(nil, nil)), create_global_frame())
    	nil
