# Lab Solution: AWS Cost Explorer and Cost Optimization

**Student Name:** Guangzheng Li  
**Date:** 24/04/2026  
**Lab Completion Time:** ___________ minutes

---

## Part 1: Cost Explorer Setup

### Screenshot 1: Cost Explorer Dashboard
![Cost Explorer](screenshots/01-cost-explorer-dashboard.png)

**Date Cost Explorer enabled (if new):** ___________________________

**Account has usage history:** ☐ Yes ☐ No (If no, practiced with interface)

---

## Part 2: Historical Spending Analysis

### 6-Month Cost Trends

**Screenshot 2: 6-Month Trend**
![6-Month Trend](screenshots/02-6-month-trend.png)

**Total spend (last 6 months):** $3,125.67

**Average monthly:** $520.94

**Highest month:** October 2025, $843.85

**Reason for highest month:**
```
EC2-other

```

---

### Daily Cost Analysis

**Screenshot 3: Daily Analysis**
![Daily Costs](screenshots/03-daily-costs.png)

**Observations about daily patterns:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

---

## Part 3: Service-Level Analysis

### Top Cost Drivers

**Screenshot 4: Top Services**
![Top Services](screenshots/04-top-services.png)

**Top 5 Services:**
1. EC2-Other: $440.39
2. Tax: $146.45
3. VPC (Virtual Private Cloud): $86.46
4. EC2-Instances: $85.26
5. Elastic Load Balancing: $45.72

---

### EC2 Cost Breakdown

**Screenshot 5: EC2 Breakdown**
![EC2 Costs](screenshots/05-ec2-breakdown.png)

**Most expensive instance type:** t3a.2xlarge

**Total EC2 cost (Oct):** $$525.65 ($440.39 + $85.26)

**Percentage of total bill:** ___________%

**Usage type breakdown:**
- On-Demand: $14.66 (Oct)
- Reserved Instances: $_______________
- Spot Instances: $_______________
- Data Transfer: $_______________

---

### S3 Cost Breakdown

**Screenshot 6: S3 Breakdown**
![S3 Costs](screenshots/06-s3-breakdown.png)

**Total S3 cost:** $_______________

**Storage cost:** $_______________

**Request cost:** $_______________

**Data transfer cost:** $_______________

**Storage breakdown by class:**
- Standard: $_______________
- Intelligent-Tiering: $_______________
- Glacier: $_______________
- Other: $_______________

---

## Part 4: Advanced Filtering

### Cost by Region

**Screenshot 7: Regional Costs**
![Regional Breakdown](screenshots/07-regional-costs.png)

**Most expensive region:** ___________________________

**Cost:** $_______________

**Are you using resources in regions you don't need?**
```
_____________________________________________________________
_____________________________________________________________
```

---

### Cost by Tag

**Screenshot 8: Cost by Tag**
![Tagged Costs](screenshots/08-cost-by-tag.png)
No tags implemented yet

**Tags analyzed:** ☐ Environment ☐ Project ☐ Team ☐ None available yet

**Cost breakdown by tag (if available):**
- Tag key: ___________________________
  - Value 1: _______________, $_______________
  - Value 2: _______________, $_______________
  - Value 3: _______________, $_______________

---

## Part 5: Cost Allocation Tags

### Activated Tags

**Screenshot 9: Activated Tags**
![Cost Allocation Tags](screenshots/09-activated-tags.png)

**AWS-Generated tags activated:**
- [ x  ] aws:createdBy
- [ ] aws:cloudformation:stack-name
- [ ] Other: ___________________________

**Activation date:** April 24, 2026, 17:08 (UTC+02:00)

---

### Tagging Strategy

**Screenshot 10: Tagged Resources**
![Tagged Resources](screenshots/10-tagged-resources.png)

**Resources tagged:** _________

**Tagging Plan:**

**Tag 1:**
- Key: Environment
- Values: production, staging, development
- Purpose: _______________________________________________

**Tag 2:**
- Key: Project
- Values: web-app, data-analysis
- Purpose: _______________________________________________

**Tag 3:**
- Key: Team
- Values: team-alpha, team-beta
- Purpose: _______________________________________________

**How will these tags help with cost management?**
```
Implementing these tags allows the finance and engineering teams to categorize spending by specific projects or environments. For example, by grouping costs by the Environment tag in Cost Explorer, I can immediately see whether the Development environment is consuming more budget than expected compared to Production. This granularity is essential for accurate chargebacks and identifying resource leaks in non-production environments.```

---

## Part 6: Custom Reports

### Report 1: Monthly Service Cost Report

**Screenshot 11: Monthly Report**
![Monthly Report](screenshots/11-monthly-report.png)

**Report configuration:**
- Date range: Last 3 months
- Granularity: Monthly
- Group by: Service
- Chart type: Bar chart

---

### Report 2: Top 10 Services

**Screenshot 12: Top Services Pie Chart**
![Top Services Pie](screenshots/12-top-services-pie.png)

**Top 3 services from pie chart:**
1. ___________________________: _______%
2. ___________________________: _______%
3. ___________________________: _______%

---

### Report 3: Daily Cost Monitor

**Screenshot 13: Daily Monitor**
![Daily Monitor](screenshots/13-daily-monitor.png)

**How often will you review this report?**
```
_____________________________________________________________
```

---

## Part 7: Cost Anomaly Detection

### All Services Monitor

**Screenshot 14: Anomaly Detection Monitor**
![Anomaly Monitor](screenshots/14-anomaly-monitor.png)

**Monitor name:** Default-Services-Monitor

**Threshold:** $10

**SNS topic:** cost-anomaly-alerts

**Email confirmed:** ☐ Yes

---

### Service-Specific Monitor

**Screenshot 15: Service Monitor**
![Service Monitor](screenshots/15-service-monitor.png)

!!!there isn't Individual services

**Services monitored:**
- [ ] EC2
- [ ] S3
- [ ] RDS
- [ ] Other: ___________________________

---

## Part 8: Optimization Opportunities

### AWS Recommendations

**Screenshot 16: Optimization Recommendations**
![Recommendations](screenshots/16-recommendations.png)

**Top 3 Recommendations:**

**1. Recommendation:**
```
_____________________________________________________________
```
- Potential savings: $_______________/month
- Effort to implement: ☐ Low ☐ Medium ☐ High
- Will implement: ☐ Yes ☐ No ☐ Maybe

**2. Recommendation:**
```
_____________________________________________________________
```
- Potential savings: $_______________/month
- Effort to implement: ☐ Low ☐ Medium ☐ High
- Will implement: ☐ Yes ☐ No ☐ Maybe

**3. Recommendation:**
```
_____________________________________________________________
```
- Potential savings: $_______________/month
- Effort to implement: ☐ Low ☐ Medium ☐ High
- Will implement: ☐ Yes ☐ No ☐ Maybe

**Total potential savings:** $_______________/month

---

### Idle Resources Audit

**Screenshot 17: Idle Resources**
![Idle Resources](screenshots/17-idle-resources.png)

**Idle resources identified:**

**Unattached EBS Volumes:**
- Count: _____
- Total size: _____ GB
- Monthly cost: $_______________

**Unassociated Elastic IPs:**
- Count: _____
- Monthly cost: $_______________

**Stopped EC2 Instances (still incurring EBS costs):**
- Count: _____
- Monthly cost: $_______________

**Old Snapshots (>90 days):**
- Count: _____
- Total size: _____ GB
- Monthly cost: $_______________

**Total idle resource cost:** $_______________/month

---

### Reserved Instance Analysis

**Current On-Demand EC2 spend:** $_______________/month

**Consistently running instances:**
- Instance type: ___________________________
- Quantity: _____
- Hours/month: _____

**Reserved Instance Pricing Comparison:**

| Term | Upfront | Monthly | Total Annual | Savings |
|------|---------|---------|--------------|---------|
| On-Demand | $0 | $_______ | $_______ | 0% |
| 1-Year, No Upfront | $0 | $_______ | $_______ | ___% |
| 1-Year, Partial Upfront | $_______ | $_______ | $_______ | ___% |
| 1-Year, All Upfront | $_______ | $0 | $_______ | ___% |

**Recommendation:**
```
_____________________________________________________________
_____________________________________________________________
```

---

## Part 9: Cost Optimization Action Plan

### Current State Assessment

**Monthly average spend:** $_______________

**Top 3 cost drivers:**
1. ___________________________
2. ___________________________
3. ___________________________

**Cost trend:** ☐ Increasing ☐ Stable ☐ Decreasing

**If increasing, by how much?** __________% over last 3 months

---

### Action Plan

**Quick Wins (Immediate - 0-1 week):**

**1.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**2.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**3.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**Quick wins total savings:** $_______________/month

---

**Short-term (1-3 months):**

**1.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**2.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**3.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**Short-term total savings:** $_______________/month

---

**Long-term (3-12 months):**

**1.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**2.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**3.**
```
Action: ______________________________________________________
Expected savings: $_______________/month
Owner: ___________________________
Deadline: ___________________________
```

**Long-term total savings:** $_______________/month

---

### Savings Summary

| Timeframe | Total Savings/Month | Annual Impact |
|-----------|-------------------|---------------|
| Quick Wins | $_______ | $_______ |
| Short-term | $_______ | $_______ |
| Long-term | $_______ | $_______ |
| **TOTAL** | **$_______** | **$_______** |

**Percentage reduction:** __________% of current spend

---

## Part 10: Stakeholder Report

### Report Export

**Screenshot 18: Exported Report**
![Exported Report](screenshots/18-exported-report.png)

**Report format:** ☐ CSV ☐ PNG ☐ PDF ☐ All

**Report includes:**
- [ ] Executive summary
- [ ] Cost trend charts
- [ ] Top cost drivers
- [ ] Optimization recommendations
- [ ] Action plan with ROI

---

## Reflection Questions

### 1. How often should you review Cost Explorer, and why?

**Your answer:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

### 2. Why are cost allocation tags important for enterprise AWS accounts?

**Your answer:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

### 3. Describe the trade-offs between Reserved Instances and On-Demand.

**Your answer:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

### 4. What is the value of Cost Anomaly Detection?

**Your answer:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

### 5. How would you present cost optimization findings to non-technical stakeholders?

**Your answer:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

---

## Self-Assessment

**Rate your confidence (1-5):**

| Skill | Before Lab | After Lab | Growth |
|-------|-----------|-----------|--------|
| Using Cost Explorer | 0/5 | 2/5 | +2 |
| Analyzing cost trends | 0/5 | 2/5 | +2 |
| Cost allocation tags | 0/5 | 2/5 | +2 |
| Identifying optimizations | 0/5 | 2/5 | +2 |
| Reserved Instance planning | 0/5 | 2/5 | +2 |
| Cost reporting | 0/5 | 2/5 | +2 |
| Anomaly detection | 0/5 | 2/5 | +2 |

---

## Instructor Verification

**Instructor Name:** ___________________________

**Date Reviewed:** ___________________________

**All reports completed:** ☐ Yes ☐ No

**Action plan realistic:** ☐ Yes ☐ No

**Comments:**
```
_____________________________________________________________
_____________________________________________________________
_____________________________________________________________
```

**Grade/Status:** ___________________________

---

**Lab Status:** ☐ Complete ☐ Needs Revision

**Submission Date:** ___________________________
