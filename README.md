# neural-network

### Neurons 
- Basic unit of neural network 
- It takes inputs, performs certain operations on them and produces an output
![Screenshot 2024-01-08 at 1.54.23 PM.jpg](..%2F..%2F..%2F..%2Fvar%2Ffolders%2Fvj%2Fwq2w4z0916q7c_6z757qykt40000gp%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_WLe4Gj%2FScreenshot%202024-01-08%20at%201.54.23%20PM.jpg)

**This is how the neuron works**:
1. Each input is multiplied by a weight 
   1. x_1 -> x_1*w_1
   2. x_2 -> x_2*w_2
2. All the weighted inputs are added together with a bias (b): 
   1. (x_1*w_1) + (x_2*w_2) + b
3. The sum is then passed through an activation function 
   1. y = f(x_1*w_1 + x_2*w_2 + b)
   2. The activation function is used to convert an unbounded input into a predictable output 
   3. eg : the sigmoid function 

### Example : 
Assume we have a 2 input neuron that uses the sigmoid activation function and has the following parameters : 
w = [0,1], b = 4  
  
w = [0,1] => w1 = 0, w2 = 1  
  
Suppose x = [2,3]
The following occur :
(w * x) + b = ((w1 * x1) + (w2 * x2))+ b
= 0 * 2 + 1 * 3 + 4 = 7 

now, y = (w*x + b) = f(7) = 0.999
> The process of passing inputs forward to get an output is known as feedforward.

### A neural network : Feedforward
> A neural network is a bunch of neurons connected together.  
  
![Screenshot 2024-01-08 at 2.31.57 PM.jpg](..%2F..%2F..%2F..%2Fvar%2Ffolders%2Fvj%2Fwq2w4z0916q7c_6z757qykt40000gp%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_Izq9ZJ%2FScreenshot%202024-01-08%20at%202.31.57%20PM.jpg)

^^ The network has 2 inputs, a hidden layer (made up of 2 neurons - h1 and h2), and an output later of 1 neuron (o1).  
> A hidden layer is any layer between the input and output layer. (There can be multiple)  
  
**Example:**

Let's assume that the network above have the same weights (w = [0,1]), the bias b = 0, and the same sigmoid activation function. 

Now we have : 
h1 = h2 = f(w * x + b)
   = f ((0 * 2) + (1 * 3) + 0)
   = f(3)
   = 0.9526 
