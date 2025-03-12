### Module 5

#### 1. ```all-student``` request
| Tool | Before Optimizing | After Optimizing |
|------|--------|-------|
Jmeter GUI | <img width="500" alt="jmeter-all-student-request-b4" src="https://github.com/user-attachments/assets/469b43fd-c150-47f1-acc5-47a02babc4eb" /> | |
Jmeter CLI | <img width="500" alt="test-result-1-b4" src="https://github.com/user-attachments/assets/b4bd0e54-434a-4c21-94c7-f6ab508e6fff" /> | <img width="500" alt="test-result-1-after" src="https://github.com/user-attachments/assets/d3ccf21f-68f6-48de-bd9f-4aec6e9c43aa" /> |
Profiling | <img width="500" alt="profile-b4" src="https://github.com/user-attachments/assets/03a25f22-4cd8-480a-9acf-0350f77e8cc4" /> | <img width="500" alt="profile-after" src="https://github.com/user-attachments/assets/de6b3101-f140-44e8-9435-123e832d4d8b" />

Conclusion: There has been an improvement of average response time from 4810 ms to 260ms from the profiling row. 

#### 2. ```all-student-name``` request
| Tool | Before Optimizing | After Optimizing |
|------|--------|-------|
Jmeter GUI | <img width="500" alt="Jmeter GUI" src="https://github.com/user-attachments/assets/5b321f2d-a0ed-4e7f-ad14-e1aecafe77ff" /> | |
Jmeter CLI | <img width="500" alt="test-result2-b4" src="https://github.com/user-attachments/assets/e2754233-9ecc-4875-9101-0f6113cba857" /> | <img width="500" alt="test-result2-after" src="https://github.com/user-attachments/assets/c2de3e62-2291-46fd-bf45-085fd661260c" />
Profiling | <img width="500" alt="profiling-all-student-name-b4" src="https://github.com/user-attachments/assets/4636a9eb-fa39-408f-85ff-1fa39efa9b56" /> | <img width="500" alt="profiling-all-student-name-after" src="https://github.com/user-attachments/assets/6dd81924-5d63-4c8f-a533-55a998e3b3f4" /> 

Conclusion: There has been an improvement of 66.7%, with average response time reduced from 390ms to 130ms. 

#### 3. ```highest-gpa``` request
| Tool | Before Optimizing | After Optimizing |
|------|--------|-------|
Jmeter GUI | <img width="500" alt="Jmeter-GUI-gpa-b4" src="https://github.com/user-attachments/assets/eab51c60-1f9b-4436-86e2-6c2e22a1524f" /> | |
Jmeter CLI | <img width="500" alt="test-result3-b4" src="https://github.com/user-attachments/assets/cfd49820-ddf2-4ab2-83d2-c609a541e64c" /> | <img width="500" alt="test-result3-after" src="https://github.com/user-attachments/assets/7d46a063-7499-467b-b7a5-77375e7d515a" />
Profiling | <img width="500" alt="highest-gpa-b4" src="https://github.com/user-attachments/assets/a2a77e34-4e0c-4895-aede-6eba907e7230" /> | <img width="500" alt="highest-gpa-after" src="https://github.com/user-attachments/assets/da9d0dd8-f7e9-4c24-99a3-a0f6e2bacc1f" />

Conclusion: There has been an improvement of 61.5%, with average response time reduced from 130ms to 50ms. 

<details>
<summary><h3> Reflection </summary>
  
##### What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?
The difference lies between the main purpose of optimizing application performance. The performance testing with Jmeter aims to measure the overall application performance under concurrency and stress, while profiling identifies bottlenecks within the applicatoin code such as CPU usage, memory allocation, and execution time). 

##### How does the profiling process help you in identifying and understanding the weak points in your application?
It helps by detecting performance bottlenecks, by allowing profiling tools to analyze CPU, memory, disk and network usage to identify slow methods. Since it also tracks memory allocation and leaks, it helps to prevent excessive memory consumption and potential crashes. It also helped to measure improvements and make sure that optimizations made are effective. 

##### Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
Yes. I think IntelliJ Profiler is effective as it helps to identify inefficient methods in our application code. Having inefficient code means we would have longer execution time which is bad. It also reduces the potential memory leaks that can happen, which will help improve the performance and stability of the code. 

##### What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?
The main challenge was with testing the performance of the methods before optimizing because of its big dataset. I think another challenge is having too much profiling data, because since the profiler shows all the CPU allocations of all the methods and the application itself, it was little overwhelming for me to see which part I need to see to do the exercise. The solution to this was prioritzing the main methods that used the most CPU and memory. 

##### What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
I think the main benefit of using IntelliJ profiler is that since it is built-in within the IntelliJ, I don't need to install an external profiling tool. As a profiler, it allowed me to monitor CPU, memory and thread activity while running the application. With the flame graphs and call trees, it helped to visualize the execusion flow to figure out which method is inefficient easily. 

##### How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
If results from IntelliJ profiler and performance testing using Jmeter is different, I would first run more tests to confirm the inconsistencies. Then make sure that the condition of both tools are similar as having different conditions may affect the results. 

##### What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?

The strategies that can be implemented are:
- Focusing on functions or queries that consume the most CPU and memory
- Using indexing and query optimzation to improve the database performace
- Reduce loops in methods (which was done in our exercise)

To ensure functionality of the application, we can write unit tests to ensure the test coverage before making changes or compare the performace of application before and after to measure the improvements. 

</details>






