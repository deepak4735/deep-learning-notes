# Geoffrey HInton
Early backpropogation experiments that led to the paper in Nature and the adoption of backpropogation was word triplets run on the network that resulted in vectors that represented the associations between the words. At the time information like that would be represented as a semantic net or another graph structure, but the backprop net was able to create feature vectors that could be converted between a semantic net and the vector. 

Of Hinton's work he was most proud of his work with Boltzmann machines and restricted Boltzmann machines. The most interesting work was that you could pass data through a Boltzmann machine and you could take your result and feed it back into the Boltzmann machine and you would learn a new bound of features that would be better than the bound of features that you had before. 

Bradford Neil and his work on varaitional statistics. They wrote a variational Bayes paper where you could approximate the true posterior with a Gaussian distribution. 

Hinton believes that the brain has something like backpropogation, and that there may be some slight implementation details that are missing. I missed some of ths so it may be worth coming back to but Hinton believes that the brain may use a stack of autoencoders and then pass back some measurement error instead of backpropogation, Yoshua Bengio is continuing a similar line of research. 

Hinton has some work with 'fast-weights' weights that adapt and decay quickly. These can be used with a recursive call. The first model was in 1973 and in 2016 he got a paper published in NIPS.

Capsules. At the point of this interview Hinton's idea about Capsule networks continually got rejected. In cap nets there is a distributed representation where a region might represent some feature. Each of the these subsets is a capsule. Its a feature with many properties. What you can do if you have that is you can do 'rooting' by agreement. If you want to do segmentation, two different capsules with two different properties for theire respectives region they can vote and agree on the same set of paramters just one level up. This is a new way of doing agreement than in most neural nets and it could be a new and better way of doing representation with less data. Its still supervied learning but the forward pass looks a lot different. 

Variational autoencoders where you use the re-paramaterization trick are according to Hinton a really nice idea for executing unsuperivsed learning along with generative-adveserial nets. GANs are one of the biggest ideas that's new in neural nets. Sparsity and slow-fetures were highly thought of ideas that fell off in time. 

> Slow features I think is a mistake. You shouldn't go for features that don't change, you should go for features that change in predictable ways. Here's a basic way in which you model anything. You take your measurements and you apply non-linear transformations to your measurements until you get to a representation as a state vector in which it is actually linear. You don't just pretend it's linear, you find a transformation from the observable to the underlying variables wher linera operations will do the work. The general principle is to go from a higher level encoding to a linear encoding where operations are cheaper and then decoding back into the higher level. 

In the 50s Turing and Von Neumann didn't care too much for symbolic AI, ther were much more concerned with the brain. Unfortunatley they died too young. The people that followed believed that what you needed in AI were symbolic expressions of some kind, cleaned-up logic where the essense of intelligence is logic. What is happening now is that a thought is a great big vector of activity veruss a symbolic expression. What comes in is a string of words, and what comes out is a string of words. The symbolic expressionist believed that what is going on in between must then be a string of words, but Hinton doesn't see it this way. The is a really important insight into how these researchers have approached the design of the algorithms in things like hidden units. 

# Pieter Abbeel 
Most of his work is in deep reinforcement learning and robotics. At berkely he worked with making robots fold laundary. For every task he found he needed domain expertise and machine learning expertise but the breakthrough of the ImageNet competition showed that you could do possibly have accuracy without much domain knoweldge in vision, he decided to revisit reinforcement learning to look for the deep version of that. In supervised learning there is a notion of input/ ouput learning. With deep reinforcement learning there is a notion of where does the data even come from- . The deep part is the representation, but there are still many questions, the representation part is largely solved. 

A lot of the problems is getting algorithms to reason over long time horizons. Right now if you can live well for 5 minutes you can be succesful as a software agent forever. 

I think safety has a lot of challenges. Human drivers fail over a long time horizon and the data collection becomes really difficult as you need to collect negative examples, crashes. There are many examples where exploration is diffiuclt. A lot of work is still required in terms of domain expertise. Reinforcement learning now is run as the final thing, whereas Pieter wants to use it earlier, I believe, in a very compute power heavy way, basically brute forcing reward functions.   

# Ian Goodfellow
One of the turning points for Ian Goodfellow was in implementing Hinton's Deep Belief Net, where he found that neural nets seemed to make much more sense than SVM's whose asymptotics are that they get slower as you add more data or that there is less paramters that you can tune not including data. 

Most of Ian's work has had to do with generative models. IN the beginnig they were using deep belief netowrks with Boltzmann machines as the building blocks- they were finicky. Then we swithced to rectifed linear units and batch normalization and deep learning became a lot more reliable. Gans are still very ustable. 

10 years ago I felt like the biggest probelm was just getting deep learning working at all for AI related tasks. We had really good tools for simpler takss where we wanted to find patterns for hand extracted features were a human designer could do a lot of that work and then hand it off to a computer. That was good findig which adds a user would click on or different kinds of basic scientific analysis, but we really stuggled with millions of pixels in an image or a raw audio wave form. We got over that hurdle maybe five years ago- now maybe the hardest part is choosing which path to go down. Do you want to make reinforcemnt learning work or supervied learning work, are machine learning algorithms fair and are you concerned with the societal issues around AI. 

Writing good code and releasing it on github or releasing articles on archiv, a lot of times its difficult to have somethng that you think is polished enough for the scientific literature but you can get to the point of having a useful software product much earlier. 

Advesarial examples. In the past there have been issues were attackers have fooled the computers into running the wrong code and that is called application security. 

We have seen that you can not fool a machine learning algorithm nto running the wrong code- and we need to build security into machine learning now. 

# 