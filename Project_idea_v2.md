In this experiment, we consider the efficient LLM scheduling problem. This is important becasue 1) the LLM service is widely adopted by plenty of business. 2) there is a large room for optimization [Revise these two reasons here based on the context]. Thus, it's important to dynamically adjust the provisioned server based on the user demand. In the real system, the LLM request is hetergenous in both their requested resources (e.g. models) and their service level objectives. For code completing jobs, the latency is more important to gain seamingless user experience, so smaller model and mroe strict should be applied. While for document processing jobs [revise the term based on the paper], to improve accuracy and reduce hallucination, a large model is a better suit for the job. To improve the overall efficiency and reducing resource wastage, recent research efforts propose to colocate these jobs in a unified resource pool and implement dynamically right-sizing techniques. 
However, some fundamental challenges persists, caused by the user demand dynamics. First, different user demand may exhibit different temporal statistics. For instance, IW-F xxx while NIW xxx[fill in some context from the paper], which means their requested resource could change, and it's necessary to do reconfigurations and relocate the resources to facilitate these request. By unloading the model for the light workload type and loading the approperiate model for the heavy task [help me revise this with approperiate terms], we can optimize the performance for each type of workload and reduce energy waste. On the other hand, such reconfiguration comes with a switching cost.  For instance, there is a waiting time associated with the VM creataion, which create plenty of delays and siginificantly energy overhead if we constantly changing the server configuration []. Thus, the optimal configuration should examine both the instantaneous performance metric detemined by the current workload and the reconfiguration cost to avoid frequent or large reconfiguration.




to switch between different 


Second, the reconfiguration cost is neglectable

the reconfiguration 



because the user demand could fluctuate a lot and the inertia in server provisioning also create some challenges here. 

and the 


not only depends on the  determined by user demand, but also 



When

 provisioning more s




