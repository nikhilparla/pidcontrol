# pidcontrol
Lesson 12 classwork examples of the selfdriving nano degree. 

- [implementPcontroller.py]() is the first implementation of a p-controller and below is the output of it.

<img src="./pictures/p-controller_output.png" alt="output of p-controller" style="zoom:50%;" />



- [implementPDcontroller]() has the differential component added too. The robot now converges onto the reference track more smoothly. Here is the output

<img src="./pictures/pd-controller_output.png" alt="pd-output" style="zoom: 50%;" />

- [systematic_bias]() is when there is wheel misalignment. The car has the steering tyres not perfectly parallel to the x-axis. Even if the bias is in steering it manifests itslef in the Cross Traffic Error in Y direction. Output below

  <img src="./pictures/systematic-bias_output.png" style="zoom:50%;" />

- pid-controller_output is the output with the integral term added too. 

  <img src="./pictures/pd-controller_output.png" alt="pid-controller_output" style="zoom:50%;" />

- implementTwiddle is the PID controller with Twiddle algorithm implemented. Instead of setting the parameters ourselves, we generate the best possible parameter values and then pass them to control. This produces the best result out of all the ones we have seen. Twiddle is just a parameter tweaking algorithm. I found it very similar to what we do with Machine Learning. It calculates error after every iteration and tweaks the three params to get better. Here is the output -

  <img src="./pictures/twiddle_output.png" style="zoom:50%;" />