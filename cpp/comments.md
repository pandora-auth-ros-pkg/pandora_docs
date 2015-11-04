# Comments

Comments are essential for maintainability.
The most important point to remember is to explain **WHY** you are doing something,
not **WHAT** you are doing.

We use `/* */` style comments for multiple lines and `//` for one liners.

#### Unnecessary comments

Don't write what code is doing, this should be left for the code to
explain and can be easily done by giving meaningful class, variable and
method names.

For example:
```cpp
// calculates square root of given number
// using Newton-Raphson method
int abc(int a){
  double t = 0.001;
  // divide by two
  double r = a / 2;
  while ( abs( r - (a/r) ) > t ) {
    r = 0.5 * ( r + (a/r) );
  }
  return r;
}
```
The previous code was **bad**.

The following is a more readable version:

```cpp
int squareRoot(int num) {
  double threshold = 0.001;
  double root = num / 2;
  while (abs(root - (num / root)) > threshold) {
    root = 0.5 * (root + (num / root));
  }
  return root;
}
```
Another **bad** example

```cpp
// ...
if (flag)
{
  temp->setPoint(*it);
  temp->setCount(counter);
  temp->setColor(_fillColors);
  temp->setBox(_rectangles);
  _landoltc.push_back(temp);
  // do stuff
  flag = false;
}
```
#### Inline Commenting

Inline comments should be placed **only** above the code, not in the same line, not
alongside function parameters etc (see above).

The following is **bad**:

```cpp
unsigned int intensity;  // it should vary between (200, 500)
```

**Good**
```cpp
// it should vary between (200, 500)
unsigned int intensity;
```

#### Don't explain third party APIs in your code.

**Bad**

```cpp
std_msgs::Float64MultiArray imuMsg;
// ...
imuMsg.data.push_back(/*float*/latestRoll_);
imuMsg.data.push_back(/*float*/latestPitch_);
imuMsg.data.push_back(/*float*/latestYaw_);
imuMsg.data.push_back(ros::Time::now().toSec());
imuPub_.publish(imuMsg);
```

#### Doxygen

We use [doxygen](https://en.wikipedia.org/wiki/Doxygen) as our documentation generation.

The doxygen comments are places **only** in the headers.

For example:

```cpp
/**
 * @brief Returns the map occupancy probability of coordinates (x,y)
 *
 * @details The probability ranges from 0-255 (0 is occupied, 255 is free)
 * @param x [int] The x coordinate
 * @param y [int] The y coordinate
 *
 * @return char probability
 *
 * @see CrsmMap::p (if needed)
 * @bug Crashes when... (if needed)
 * @warning If x,y out of range program... (if needed)
 **/

char getMapProbability(int x, int y);
```

For more examples and HOWTOs see the doxygen [wiki](http://www.stack.nl/~dimitri/doxygen/).

#### Legal notice

Every source file should start with the following license:

```
/*********************************************************************
 *
 * Software License Agreement (BSD License)
 *
 *  Copyright (c) 2015, P.A.N.D.O.R.A. Team.
 *  All rights reserved.
 *
 *  Redistribution and use in source and binary forms, with or without
 *  modification, are permitted provided that the following conditions
 *  are met:
 *
 *   * Redistributions of source code must retain the above copyright
 *     notice, this list of conditions and the following disclaimer.
 *   * Redistributions in binary form must reproduce the above
 *     copyright notice, this list of conditions and the following
 *     disclaimer in the documentation and/or other materials provided
 *     with the distribution.
 *   * Neither the name of the P.A.N.D.O.R.A. Team nor the names of its
 *     contributors may be used to endorse or promote products derived
 *     from this software without specific prior written permission.
 *
 *  THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 *  "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 *  LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
 *  FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
 *  COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
 *  INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 *  BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 *  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 *  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 *  LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 *  ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 *  POSSIBILITY OF SUCH DAMAGE.
 *
 * Authors:
 *   John Doe <johndoe@example.com>
 *********************************************************************/
```


