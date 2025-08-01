# 🔍 JMeter Load Test - SauceDemo  
**Performance testing project** demonstrating fundamental QA skills  

## 🛠️ Technical Implementation  
- **Test Tool**: Apache JMeter  
- **Scenario**: 10 virtual users performing:  
  - Login → Browse Products → Checkout  
- **Key Challenges Solved**:  
  - Session persistence using HTTP Cookie Manager  
  - Debugged 404 errors in SPA routing  

## 📊 Results Summary  
| Metric          | Value       |  
|-----------------|-------------|  
| Throughput      | **62** req/sec |  
| Avg. Response   | **800ms**   |  
| Error Rate      | **4%**      |  

![Error Analysis](results/screenshots/error_analysis.png)  

## 🚀 How to Run  
```bash
jmeter -n -t test_plans/SauceDemo_LoadTest.jmx -l results/results.jtl
