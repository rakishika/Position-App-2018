# Position-App-iOS
Winner of Superposition Hackathon 2018 for best app iOS app



Inspiration
"Optimization is the only way to accomplish present success." With hospital spacial inefficiency being one of the leading causes of death in the United States, it is important to learn how to optimize your spaces such that important services are located at the best points of access to other stations. For example, for an architect deciding the best location to build a warehouse relative to factories, it is important to find the best place to locate this warehouse in order to minimize costs of travel and transportations. More importantly, bad location of hospital emergency services being one of the leading causes of death, it is important to find the best location for surgical equipment and emergency services relative to points of access.

What it does
This app uses Weiszfeld's algorithm. This particular algorithm takes an arbitrary point a. Then, each of the points which are desired for optimization can be defined as a_1, a_2, a_3, ..., a_n. Then, take the a_1/(distance from a to a_1) + a_2/(distance from a to a_2) + ... + a_n/(distance from a to a_n). Divide this value by the sum 1/(distance from a to a_1) + 1/(distance from a to a_2) + ... + a_n/(distance from a to a_n). The resulting point p is the next approximation. From there, repeat the algorithm, except replace a with p. This algorithm repeats until you get a point q that converges, which is then the point that minimizes the sum of the distances to this point from the other points. Using a code of this algorithm with 500 iterations, the app quickly calculates the geometric median of a set of points, meaning the point that minimizes the sum of this point to the other desired location points. The user can input a set of points by pressing on a specific coordinate plane and then see their geometric median.

How we built it
We used swift and objective-c to code the app on XCode, which shows how the storyboard for the app would work. Because of XCode's developing state and thus inability to incorporate the click-to-show program, we have incorporated a program in Java which represents the geometric median. Additionally, a website for promotional purposes was coded using CSS, JavaScript, and HTML. Finally, the website contains a JotForm which is programmed to accept donations through the Stripe software.

Challenges we ran into
The main challenge we ran into was incorporating the Java code onto the XCode platform. This was the main challenge because the XCode software, which is still in developing stages, did not have a straightforward integration of a touch-to-click program. Therefore, we used a Java program to calculate the geometric mean with a user just clicking points to represent where their objects are located.

Accomplishments that we're proud of
We are proud of coding the Java program which worked way better than what we expected. We were able to have a loop that runs 500 iterations of the algorithm, resulting in a point which converges to the geometric median of a set of points. Initially, we thought the user would have to physically type out the coordinates of their points of location, but we were able to have the program work by the user just clicking the locations of their objects. Additionally, we are extremely proud of incorporating a complex mathematical algorithm, the Weiszfeld's algorithm, into this program.

What we learned
This was our first time coding in Java Swing and using the GUI interface to make a program. Therefore, we were able to learn how to incorporate user actions, such as the MouseListener, into arrays that displayed mathematical functions. This app helped us learn that computer science is not only restricted to that itself, it can incorporate many other subjects, such as math.

What's next for Position: An implementation of Weiszfeld's Algorithm
We hope to incorporate the Java code onto an iOS app for tablets in order to help architectures, interior designers, and even the every day person in order to best make use of the space we're given.

Built With
css
html
java
javascript
objective-c
swift
xcode
