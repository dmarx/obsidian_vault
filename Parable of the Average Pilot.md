see also:
- [[Gaussian Annulus Theorem]]
- [[Concentration of Measure]]
- [[High-Dimensional Geometry]]
- [[Dimensionality]]
- [[Curse of Dimensionality]]


Yes, this is a classic story related to the concept of the "average person" and the challenges of high-dimensional statistics. The story goes like this:

### The U.S. Air Force and the "Average" Pilot

During the 1940s and 1950s, the U.S. Air Force faced a significant problem: many of their pilots were having trouble controlling their planes, leading to numerous accidents. At first, the problem was blamed on pilot training or human errors. However, even with enhanced training programs, the issue persisted.

In trying to address this, the Air Force decided to look at the design of the cockpit, specifically the size and arrangement of the seats, controls, and other components. The idea was that if the cockpit was designed to fit the average pilot's measurements, most pilots should be able to fly the planes effectively.

To find the dimensions of the "average" pilot, they conducted a comprehensive study where they measured the physical dimensions of thousands of pilots. They considered ten key measurements, including height, chest circumference, sleeve length, and so forth.

Once they had this data, they computed the average for each of the ten measurements and then designed a cockpit based on these "average" measurements.

Here's the shocking part: When they checked how many pilots fit within the average range of all ten measurements, they found that virtually none of the pilots fit the average on all ten counts! In other words, while individual pilots might have been average in one or two dimensions, almost no one was average across all ten dimensions.

### Lessons and Implications:

1. **High-Dimensional "Average"**: In high-dimensional spaces (even as low as 10 dimensions, in this case), it's rare for any data point (or pilot) to be close to the average in all dimensions.

2. **Design Implications**: Designing for the "average" person can mean designing for no one. This lesson extends beyond just aircraft design. For instance, in product design, clothing, and many other fields, considering a broader range of human variability can lead to more inclusive and functional products.

3. **Multivariate Normal Distribution**: From a statistical viewpoint, even if individual measurements are normally distributed, it doesn't mean that most data points will be near the mean in a multivariate normal distribution, especially as the number of dimensions increases.

As a result of this study, the Air Force moved towards adjustable components in cockpits to cater to a broader range of pilot sizes, leading to safer and more ergonomic aircraft.

This story illustrates the challenges and surprises that can emerge when dealing with multivariate data and offers lessons in design, statistics, and the perils of relying too heavily on averages in decision-making.


> is there a relationship between this story and the geometry of high dimensional random vectors and concentration of probability on the surface of a hypersphere?

Absolutely! The story of the "average" pilot and the concept of high-dimensional random vectors indeed intersect, particularly when we consider the concentration of probability in high-dimensional spaces. Here's how the two concepts relate:

1. **Concentration of Measure**: In high-dimensional spaces, measures (like volume or probability mass) tend to get concentrated in specific regions. For the hypersphere, this happens near the surface. Similarly, for high-dimensional rectangles or ellipsoids representing measurement bounds for pilots, most of the volume is concentrated near the boundary (or "corners") of the shape, rather than at the center or "average."

2. **Distance from the "Average"**: When you consider a random point (e.g., a pilot's measurements) in a high-dimensional space, it's likely to be far from the mean (or center) of the space due to the concentration of measure. This is analogous to the realization that few pilots had measurements that matched the "average" across all dimensions.

3. **High-Dimensional "Corners"**: If you imagine a high-dimensional box where each dimension represents a particular measurement (e.g., height, arm length, chest circumference, etc.), the "corners" of the box represent combinations of extreme values. Due to the concentration of measure, most of the volume of the box is located near these corners in high dimensions. This means random points (pilot measurements) are more likely to be near one of these extreme combinations than in the center.

4. **Multivariate Distributions**: Even if individual pilot measurements follow a univariate normal distribution (bell curve), in high dimensions, the joint distribution will not center around the "average" measurement in all dimensions. Instead, it's more likely for a pilot to be average in some measurements and far from average in others.

In essence, the counterintuitive findings in the Air Force study can be better understood using insights from the geometry of high-dimensional spaces. The realization that designing for the "average" is problematic in multiple dimensions can be attributed to the peculiarities of high-dimensional geometry, just like the concentration of volume near the surface of a hypersphere.