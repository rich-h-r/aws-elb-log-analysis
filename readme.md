# Details

Simple tool to analyse AWS Elastic Load Balancer Logs.

## TODO: 
1. this works for classic loadbalancers, Application and Network Load balancers have different fields in the logs.
2. create a plot to show the differences in loads between weeks

## checking in the notebook to git
clear all the output from notebook by selecting from the notebook menu Cell > All Output > Clear

## Getting started

1. Create a new virtual env to host the notebook
```
$ python3 -m venv ~/virtual_envs/jupyter_elb_log_analysis
```
2. activate the virtual environment
```
$ source ~/virtual_envs/jupyter_elb_log_analysis/bin/activate
```
3. restore all the dependencies
```
$ pip3 -r requirements.txt
```
4. run the jupyter nodebook
```
$ jupyter notebook aws-elb-log-analysis.ipynb
```
###notes:
this uses your default aws profile found in `~/.aws`, you will have to alter the boto3 command, or set the `AWS_PROFILE` environment variable to a suitable profile


