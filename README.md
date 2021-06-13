# thread-safe-counter

L1-5 : Add Source File

L7-10 : Declares a type (pthread_mutex_t) for storing mutex information.

L12 : unsigned int value loop_cnt value definition

L15-18 : pthread_mutex_init is used to initialize the mutex object, the first factor initializes the object mutex, and the second factor uses attr to change the mutex attribute (where NULL is used to use the default attribute).

L20-24 : in pthread_mutex_lock(&c->lock) means the start of a critical section, and pthread_mutex_unlock(&c->lock) means the end of a critical section. c->value++ increased a value by one.

L26-30: <decrement>c->value—reduced one value. pthread_mutex_lock (&c->lock) means the start of a critical section, and pthread_mutex_unlock (&c->lock) means the end of a critical section.

L32-37: Access to rc to members of structure c pointer

L39-50 : Increments the counter address by repeating string memory addressing & output, loop_cnt. String address output when finished
  
L52-67 : defines the value of transforming the string of characters in argv[1] into integers (atoi). Run until &counter's value is terminated. Define p1 and p2 for storing mutex information.
pthread_create creates threads. The first parameter is the thread identifier used to identify the fishy threads when the threads are successfully created. The second parameter, attr, is used to specify thread properties, and NULL is used to exploit the default thread properties. The third parameter, start_routine, is a thread function to branch out, and the fourth parameter, arg, is passed to the parameter of the above start_routine thread function.
Pthread_join waits for a particular thread to terminate, and then proceeds to: The first parameter is the identifier of the thread to wait for, and the second parameter is the return value of the thread.
Finally, I print out the results.
