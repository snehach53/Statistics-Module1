**Probability Basics**

Today I learnt about Probability basics, Random variable, Types of
random variable (continuous and discrete), Sample space , Population,
Sample, Random experiment, basic outcome, event, probability mass
function, Probability density function I would to like to implement
Restaurant chain "Hunger Pangs" as a real-world use case.

1.  **Probability Basics**

Probability is the measure of how likely something is to happen.

It's like a number that tells you:

-   If something is impossible → probability is 0.

-   If something is certain → probability is 1.

-   If something might happen → probability is a number between 0 and 1.

Probability in Machine Learning is used to model uncertainty in data,
predictions, and model behavior.

**Mathematical formula: No. of Desired outcomes / Total possible
outcomes**

2.  **Random Experiment**

**Definition**: A process with uncertain outcomes but a defined set of
possible results.

**Example:** Observing whether each customer at hunger pangs orders a
dessert or not.

Here, the random experiment is **watching the behavior** (Customer
having dessert or no dessert), you know the possible outcomes, but you
do not know what will happen each time.

3.  **Random Variable**

A numerical value assigned to outcomes of a random experiment. It
represents measurable outcomes.

**Use Case Example**: Counting how many customers out of 10 order a
dessert. Here, the random variable is **the number** (like 3, 5, or 7)
of customers who ordered dessert , it turns the observation into a
countable, numeric result.

4.  **Types of Random Variable**

**Discrete Random Variable**: Takes countable values (**Finite
outcomes**) (integers like 0, 1, 2).

**Example**: Number of orders placed in a day at Hunger pangs , Suppose
10 orders placed .

**Continuous Random Variable**: Takes any value in a range (Infinite
Outcomes within a range)

**Example**: Time taken to serve a customer.

5.  **Sample Space**

**Definition**: The set of all possible outcomes of a random experiment.

**Experiment:**\
To Observe the type of meal a randomly selected customer orders at one
of the restaurant's locations.

**Possible outcomes**

-   Breakfast

-   Lunch

-   Dinner

-   Snack

-   No order (just browsing!)

**Sample Space (S):**

S= {Breakfast, Lunch, Dinner, Snack, No order}

**Example**:

6.  **Population**

**Definition**: The entire group of items or individuals being studied.

Here the group of customers visiting the Hunger pangs at all locations

**Example**: All customers visiting a restaurant chain Hunger pangs
globally.

7.  **Sample**

**Definition**: A subset of the population selected for analysis.

**Example**: Customers visiting one specific restaurant branch on a
given day, Used for studying and analyzing the behavior of customers at
a particular location or branch.

8.  **Basic Outcome**

**Definition**: A single possible result of a random experiment.

**Example**: The first customer of the day orders a vegetarian meal.

This is a **basic outcome** because it is one, well-defined result from
all the possible things that could happen.

9.  **Event**

**Definition**: A specific outcome or set of outcomes from a random
experiment.

**Example**: At least one customer orders a dessert during lunch hour.

This is an event because it's a particular outcome I'm interested in
among all possible combinations of customer orders; I am focusing on the
cases where someone orders dessert.

10. **Probability Mass Function (PMF)**

**Definition**: A function that gives the probability of each possible
value of a **discrete** random variable.

**Formula**: The PMF is written as:

P(**X**=x)
=Probability that exactly x customers order dessert in an hour

**Example values:**

> P(X=0) → probability no one orders dessert.
>
> P(X=5) → probability exactly 5 people order dessert.
>
> P(X=10) → probability exactly 10 people order dessert.
>
> **All probabilities are non-negative**:
>
> ![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image1.png){width="2.257060367454068in"
> height="0.2777919947506562in"}
>
> **The sum of all possible probabilities equals 1**
>
> ![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image2.png){width="2.2778947944006998in"
> height="0.6319772528433946in"}
> ![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image3.png){width="3.6220089676290463in"
> height="3.6772747156605425in"}

**Example**: Here I'm modeling the probability that 0--10 customers
order dessert in an hour at the restaurant.

We can Notice how the highest probabilities are around 4--6 customers,
and the bars represent the **probability mass** for each discrete
outcome.

![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image4.png){width="4.2981485126859145in"
height="2.809248687664042in"}

11. **Probability Density Function (PDF)**

**Definition**: How the probabilities are spread across all possible
outcomes of a random variable. The probability is found by integrating
the PDF over that range.

Now we are looking at

Random variable Y → **amount of money a customer spends on dessert per
visit** at restaurant

**Possible values:**

Any real number between \$0 and \$20\
This makes it a **continuous** random variable.

Lets say P( 4\<=Y\<=6 ) is 0.25

This means:

There is a **25% chance** that a randomly selected customer spends
between \$4 and \$6 on dessert.

![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image5.png){width="5.546590113735783in"
height="3.5549136045494314in"}

The **purple curve** → the probability density over dessert spending
(centered around \$10, spread across \$0--\$20).

The **shaded area between \$4 and \$6** → the actual probability
P(4≤Y≤6) which comes from integrating (calculating the area) under that
section of the curve.

**Cumulative Distribution Function**: Probability that the random
variable **Y** is **less than or equal to** a specific value" y"

![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image6.png){width="2.465404636920385in"
height="0.6111428258967629in"}![](vertopal_937891a0cb8d484badc6453c11c482e4/media/image7.png){width="6.236431539807524in"
height="0.902823709536308in"}

If we subtract:

F(6) − F(4)

We remove everything below \$4 and are **left only with the part between
\$4 and \$6**.
