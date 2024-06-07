# helm

How to create a Helm Chart ?

1) First create an empty chart
    $ helm create chartName 

2) Componets that you need tempaltized has to be present on templates/ 

3) Based on the environment, you'd supply env-values.yaml 

4) First you install the chart and from the next time whenever there is a change in the values, you go woth udpate.
    # helm install -f values.yaml . 

    # helm upgrade -i -f values.yaml .