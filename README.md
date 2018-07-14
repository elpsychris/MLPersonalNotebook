# MY PERSONAL NOTEBOOK
My notebook of exercises, blogs and related resource I read in free time
## 1. NN and Deep Learning - By Michael Nielsen

### [1.1. Chapter 1](http://neuralnetworksanddeeplearning.com/chap1.html)

#### 1. Perceptrons
- [ ] demo project
- [ ] note
- [ ] doing exercise
  ##### 2.b. Note
0. What is a **Perceptrons**:

* A type of Artificial neuron
* Developed in 50s and 60s by Frank Rosenblatt

1. How it work?
 

#### 2. Sigmoid neurons
- [ ] demo project
- [ ] note
- [ ] doing exercise
  ##### 2.c. Exercise
1. Sigmoid neurons simulating perceptrons, part I  

**Suppose we take all the weights and biases in a network of perceptrons, and multiply them by a positive constant, c>0. Show that the behaviour of the network doesn't change.**
```
ANSWER:

- According to the concept, the output value of a NoP is:
  * 0 if Sum of (wj)(xj) <= *threshold*
  * 1 if Sum of (wj)(xj) > *threshold*

  Therefore if before value is 0, new value is still 0*c = 0 and the same with 1
```
2. Sigmoid neurons simulating perceptrons, part II

Suppose we have the same setup as the last problem - a network of perceptrons. Suppose also that the overall input to the network of perceptrons has been chosen. We won't need the actual input value, we just need the input to have been fixed.
```
ANSWER:

- Delta(output) is a linear function of changes Delta(wj) and Delta(b),
hence when c comes to infinity (c>0) the output value will tend to 0 if z < 0
and tend to 1 if z > 0. The same thing happened with the perceptrons.
```

Suppose the weights and biases are such that (wj)x+b != 0 for the input x to any particular perceptron in the network. Now replace all the perceptrons in the network by sigmoid neurons, and multiply the weights and biases by a positive constant c>0. Show that in the limit as c¨inf. the behaviour of this network of sigmoid neurons is exactly the same as the network of perceptrons. How can this fail when (wj)x+b=0 for one of the perceptrons?

```
ANSWER:

- For the signoid when z = 0 => output = 1 / 1 + e^0 = 0.5 !== 0 in the perceptrons case,
hence leads to different behavior afterward. 
```

