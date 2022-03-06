## <p align=left> Highly Available Microservices Architecture Deployment Solution <br> <br> </p> 

| **SL** | **Topics** |
| --- | --- |
| 01 | [My Opinion](#01) |
| 02 | [Cloud Native Architecture](#02) |
| 03 | [Architecture Evolution](#03) |
| 04 | [Infrastructure as Code (IaC)](#04)  |
| 05 | [Loadbalancing, Single Point of Failure, Scalability, Fault Tolerance, Auto Recovery Considerations](#05) |
| 06 | [CI/CD Strategies and Tool Justification along with Test Automation](#06)|
| 07 | [Infrastructure Monitoring System](#07)|
| 08 | [Secret Management](#08)|
| 09 | [Why Cloud-Native Architecture?](#09)|
| 10 | [Advantages of Why Cloud-Native Architecture](#10)|

### <a name="01">My Opinion</a>
In my opinion cloud native architecture will be best highly available microservices architecture.

### <a name="02">Cloud Native Architecture</a>
Cloud-native architectures are those that take advantage of the things that cloud platforms do well. For example, it is easy to scale out a cloud-based application by simply adding more server nodes, as well as to scale back down if the scale-up was due to a temporary spike in demand. So cloud-native applications should provide horizontal scaling capability, and not be monolithic apps that are deployed on a single server. This is done in part by adopting a microservices architecture, where the app is decomposed into small functional pieces that can be deployed independently and connected via stable, clearly defined APIs.   

<img src= "https://github.com/Shadikul-Islam/DevOps-Test/blob/master/Task-03/Images/Image1.png" alt="Cloud Native Architecture">

### <a name="03">Architecture Evolution</a>
For the last 50 years or so, software architecture and application hosting models have experienced major transformation from mainframes to microservices and serverless.
Below Image shows this evolution of architecture models and the paradigms they promoted.
<img src= "https://github.com/Shadikul-Islam/DevOps-Test/blob/master/Task-03/Images/Image2.png" alt="Cloud Native Architecture">

### <a name="04">Infrastructure as Code (IaC)</a>
IaC is the managing and provisioning of infrastructure through code instead of through manual processes.
With IaC, configuration files are created that contain your infrastructure specifications, which makes it easier to edit and distribute configurations. It also ensures that you provision the same environment every time. By codifying and documenting your configuration specifications, IaC aids configuration management and helps you to avoid undocumented, ad-hoc configuration changes.

These are a few popular choices:
- Chef
- Puppet
- Red Hat Ansible Automation Platform
- Saltstack
- Terraform 
- AWS CloudFormation

In my opinion if we use AWS then we can use **AWS CloudFormation** otherwise we can use Terraform for open source infrastructure as code software tool.

### <a name="05">Loadbalancing, Single Point of Failure, Scalability, Fault Tolerance, Auto Recovery Considerations</a>
To handle all of these we can use **Kubernetes** service. Kubernetes can handle all of those things very easily. Kubernetes is an open source container orchestration platform that automates many of the manual processes involved in deploying, managing, and scaling containerized applications.

<img src= "https://github.com/Shadikul-Islam/DevOps-Test/blob/master/Task-03/Images/Image3.png" alt="Cloud Native Architecture">

### <a name="06">CI/CD Strategies and Tool Justification along with Test Automation</a>
There are a lot of CI/CD and Test Automation tools in the market. I think **Jenkins** will be good to handle the CI/CD Strategies and Tool Justification along with Test Automation. Jenkins is a server-based application and requires a web server like Apache Tomcat to run on various platforms like Windows, Linux, macOS, Unix, etc. To use Jenkins, you need to create pipelines which are a series of steps that a Jenkins server will take

### <a name="07">Infrastructure Monitoring System</a>
We can use **Nagios**. Nagios is one of the most popular free and open-source DevOps monitoring tools. It helps you monitor your infrastructure to find and fix problems. Nagios Core is a command line tool, Nagios XI provides you with a web-based GUI (graphical user interface) and monitoring wizard, Nagios Log Server lets you search log data and set up alerts about potential threats.

### <a name="08">Secret Management</a>
Secret Management is an integral part of secure software development and infrastructure automation. If our cloud provider is AWS/Azure/Google then we can take their Secret Management tools like AWS Secrets Manager/Microsoft Azure Key Vault/Cloud KMS. For open source tool, **Strongbox** will be good as per my opinion.

### <a name="09">Why Cloud-Native Architecture?</a>
A cloud-native architecture uses containers, microservices, development and operations DevOps tools, and many third-party components to optimize your development, testing and O&M efforts. This reduces the complexity of managing distributed systems and accelerates your business iteration, freeing up your developers to focus on value-added tasks.

### <a name="10">Advantages of Why Cloud-Native Architecture</a>
**High Availability**: A cloud-native architecture can provide high availability in both your primary/secondary and cluster modes, and cold backup, with a switchover of a few seconds and providing services that feature more than 99.999% availability.

**Capacity Evaluation**: Our Application Real-Time Monitoring Service (ARMS) can evaluate both the capacity of a single machine and the overall capacity of your system. As a result, you can make accurate resource plans and cost estimates for both your future promotions and ongoing business, helping you autonomously scale with confidence.

**Stability Assurance**: If your organization holds regular promotions, this can cause peaks in demand across your network. Our cloud-native architecture recently helped the Double 11 2020 Shopping Festival reach a total transaction amount of 498.2 billion RMB in just 24 hours, handling 583,000 orders per second at its peak.

**Cost Effectiveness**: Most Cloud provider offer pay-as-you-go or subscription payment model. If you decide to subscribe, then you can realize economies of scale and, if you choose pay-as-you-go, then you do not need to pay a large amount of money in advance for your servers and racks.

**High Efficiency**: A cloud-native architecture also centralizes your O&M, using a continuous integration process that involves initializing projects based on business requirements, pulling code from a specified branch to develop applications, performing regression testing in the test environment, verifying applications in the staging environment, and publishing applications.

**Automation**: Automation can help further reduce the complexity and scale of your software technology across your cloud-native architecture. For example, our Infrastructure as Code (IaC), GitOps, an Open Application Model (OAM), Kubernetes operators, and various automated delivery tools can be used to implement Continuous Integration (CI) and Continuous Deployment (CD)





