# Drone Operator Behavior Models through HMM
This is the code for develeping human operator behavior models through Hidden Markov Model(HMM), to further study the impact of operators’ drone control strategies as a function of differing levels of autonomy. Details are shown in the paper "The Impact of Different Levels of Autonomy and Training on Operators’ Drone Control Strategies".

## Requirement
MatLab is required to run the code.

## Developing HMM model in this project can be split into two steps.
### Choose the number of hidden states (plot BIC)
In MatLab command window, Run 

plotBIC( path, num_ob_states ) 

### Model Selection
In MatLab command window, Run 

\[Log_Liks, Trans, Emis, Freqs ] = selectModel( path, num_ob_states, num_hidden_states )

then select the model based on Log Likelihood, Transition Probabilties and Emission probabilties.
