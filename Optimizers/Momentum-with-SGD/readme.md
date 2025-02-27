research paper - https://paperswithcode.com/method/sgd-with-momentum#:~:text=due%20to%20momentum.-,Suppose%20we%20have%20a%20starting%20point%20A%20and%20want%20to,idea%20behind%20SGD%20with%20Momentum.

SGD - Stochastic Gradient Descent

# **Momentum**

In deep learning, "momentum optimization" is a technique that improves the convergence speed of gradient descent algorithms by accumulating information from past gradients, essentially creating inertia to move more smoothly towards the global minimum, reducing oscillations and allowing for faster learning, especially in complex loss landscapes with many local minima and saddle points; it's like adding "momentum" to a ball rolling downhill, making it accelerate in the correct direction instead of getting stuck in small dips and turns. 

![image](https://github.com/user-attachments/assets/8f69aa1c-f63d-412c-b0fe-f7a27c83a855)


* Momentum prevents stalling of the optimization process that is much more likely to occur for stochastic gradient descent.

* The effective number of gradients is given by 1/(1-B) due to exponentiated downweighting of past data.

**Key points about momentum optimization**

**How it works**

Instead of relying solely on the current gradient to update parameters, momentum incorporates a fraction of the previous update direction, effectively smoothing out the update path and pushing the model towards the optimal solution faster. 

**Mathematical intuition**

* **Velocity term:** 
A "velocity" variable is introduced to store the exponentially weighted average of past gradients. 

* **Update equation:**
When updating parameters, the current gradient is added to the scaled velocity term, giving more weight to recent gradients. 

**Benefits**

* **Faster convergence:**
Momentum significantly reduces the number of training iterations needed to reach a good solution. 

* **Reduces oscillations:**
By averaging out noisy gradients, momentum helps avoid getting stuck in local minima or oscillating between different directions.

* **Better handling of saddle points:**
In regions with flat gradients (saddle points), momentum can provide a direction to move towards the global minimum. 

**Hyperparameter**

* **Momentum coefficient (β):**
Controls how much influence past gradients have on the current update. A higher β means more emphasis on past gradients, potentially leading to faster convergence but also risking overshooting the optimal point. 

**Example application**

Imagine a ball rolling down a bumpy hill: Without momentum, the ball might get stuck in small dips and take a long time to reach the bottom. With momentum, the ball gains speed as it rolls, allowing it to easily overcome small obstacles and reach the bottom much faster. 
