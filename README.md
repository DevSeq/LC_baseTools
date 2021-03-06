# LC_baseTools
Tools to make programming Arduinos easier.

**blinker** - Blinks an LED without using delay(). Or any output pin for that matter. Does NOT use interrupts or hardware PWM.

**colorObj** - Used for everything dealing with colors. Storing, translating, passing from computer to hardware and back. Blending, linear and non-linear color mapping.

**debug** - Grab bag of debugging tools. Includes ST (Stack trace). Put ST at the start of a function. Then, that function's name prints on the serial monitor when executed.

**idlers** - Contains the idler class used to make objects that function in the background. Also includes the support code to make this happen automatically.

**lists** - Base classes of dynamic linked lists that everything in the LC libraries are based on. Linked Lists, double linked lists, stack and queue.

**mapper** - Linear mapper function. Unlike the Arduino version, this uses doubles as input and output. It also saves as much of the calculation as possible between mapping calls.

**mechButton** - Class that creates a debounced button. It works, its in need of a rewrite.

**multiMap** - Non-linear mapping function. Starts out blank and the user adds x,y points to it before use.

**resizeBuff** - Simplified memory management. Initialize your pointers to NULL then resizeBuff() can allocate and deallocate your dynamic buffer space for you. Passes back true for successful allocations, false for unsuccessful. Saves a lot of code typing.

**runningAvg** - Running average data smoother. Pop in a number, and out popes the average of the last n numbers inputted.

**squareWave** - Base class for creating objects that are based on square waves. IE. blinking lights, flashing text, RC servo signals. Does NOT use interrupts or hardware PWM. Runs in background.

**textBuff** - Ring buffer for text. Handy for hardware that can pass in a lot of text at random times that you need to process. 

**timeObj** - A timer that takes a Ms input as a float. Then it can be queried to tell when this timespan has expired. Takes care of roll over issues as well. Very handy for getting away from delay(). Set a timer, and let loop() run. When it expires, do your thing.
