# Project Title: Application of Machine Learning to Solve the Inverse Problem of Envelope Equations in Accelerator Physics
We are working on solving the inverse problem of the Kapchinsky-Vladimirsky (KV) envelope equation in accelerator physics expressed as

$$
r_x'' + kr_x - \frac{2K}{(r_x+r_y)}-\epsilon_x^2/r_x^3= 0 
$$

$$
r_y'' - kr_y - \frac{2K}{(r_x+r_y)}-\epsilon_y^2/r_y^3= 0 
$$

Where $r_x$ and $r_y$ are the horizontal and vertical beam envelope radii as functions of the position  $𝑠$ along the beamline. $\epsilon_x$ and $\epsilon_y$ are the horizontal and vertical emittances, representing the beam's spread in phase space. The parameter $k$ is the external focusing strength (e.g., from magnetic lenses). And last parameter $K$  accounts for the space charge effect, which causes beam expansion due to the repulsive forces between charged particles. In this project, we intend on using: Machine learning, Physics-Informed Neural Networks (PINNs), Non-linear regression. The goal is to infer parameters or conditions of the KV equation from observed or simulated data.
