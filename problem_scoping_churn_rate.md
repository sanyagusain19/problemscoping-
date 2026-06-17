# 🛒 E-Commerce Churn Rate Problem Scoping

## 📌 Executive Summary

This document outlines a comprehensive problem framing for an **AI/ML project aimed at reducing customer churn** in an e-commerce platform. A **critical 10% increase in churn rate (28% → 38%) over 6 months** signals an urgent need for data-driven investigation and intervention.

---

## 🔍 1. Uncover the Problem

### Current State
- **Current Churn Rate:** 28-30%
- **Recent Peak:** 38% (6 months ago)
- **Increase:** 10% jump in churn rate within 6 months
- **Signal:** Critical inflection point requiring immediate action

### Key Questions
- ❓ What is the current churn rate? → **28-30%**
- ❓ Which type of customer has high churn?
- ❓ Since when did it increase drastically? → **6 months, with slight shifts noticed before**

### 💡 Key Insight
> A 10% jump in churn rate (28% → 38%) within 6 months signals a **critical inflection point** requiring immediate data-driven investigation.

---

## 🛠️ 2. To Technical Department

### Technical Questions
- What changes were made after which churn rate increased abruptly?
- Have you made any changes in app architecture or delivery pattern within these 6 months?
- Any pricing or discount strategy changes?

### 📅 Suspected Changes Timeline

| Timeline | Change | Impact Level |
|----------|--------|--------------|
| **5 months ago** | Payment gateway update | 🔴 High |
| **4 months ago** | App UI redesign + Delivery partner change | 🔴 High |
| **3 months ago** | Discounts reduced, competitor increased offers | 🔴 High |

---

## 💼 3. To Management - Why This Problem Matters?

### Business Impact

| Impact Area | Details |
|-------------|---------|
| **Revenue Direct Contact** | Churn directly reduces revenue and customer lifetime value |
| **Market Position** | High churn in competitive market = risk of being overtaken |
| **Investor Confidence** | High churn is a red flag for unsustainable growth |
| **Growth Sustainability** | If churn remains high, company faces a "hideous situation" |

### 📊 Key Business Metrics

- 🎯 **Acquisition Cost:** New customers cost **5x more** than retaining existing ones
- 📉 **CLV Impact:** High churn = reduced Customer Lifetime Value
- ⚠️ **Investor View:** High churn signals unsustainable growth model
- 💰 **Revenue Risk:** Each lost customer = lost recurring revenue

---

## 🎯 4. Better Approach - Problem Definition

### Who, What, Why, Outcome

| Element | Description |
|---------|-------------|
| **Who** | Customers facing problems (at-risk of churning) |
| **What** | Predict which customers will churn |
| **Why** | Enable company to take preventive actions (discounts, coupons, support) |
| **Outcome** | **8-10% decrease** in overall churn rate |

### Target Customer Segments
- 🔵 New customers (higher churn risk)
- 🔵 Inactive customers (>60 days without activity)
- 🔵 Tier 2 customers (price-sensitive)
- 🔵 Customers with delivery/service issues

### Retention Actions
- ✅ Targeted discounts & coupons
- ✅ Personalized offers based on behavior
- ✅ Improved customer support
- ✅ Re-engagement campaigns

---

## 🤖 5. Is AI Really Needed?

### ✅ Where AI Adds Value

**AI should be used for:**
- 🧠 Finding complex patterns in customer behavior
- 👥 Customer segmentation and targeted offers
- 📈 Generating actionable insights
- 🎯 Churn detection and risk scoring

**AI cannot be replaced by simple rules** because churn depends on:
- 📍 Customer type and geographic location
- 💬 Customer service quality
- 💵 Cost-to-utility perception
- 🔄 Evolving customer needs

### ❌ Why Simple Rules Fail

**Simple Rule:** "If inactive for 60 days = churned"

**Problem:** Misses complex patterns like:
- ✖️ New Tier-2 city customers
- ✖️ With previous delivery delays
- ✖️ Who accessed app after UI update
- ✖️ During competitor promotion period

**Solution:** AI detects these **multi-factor combinations** that humans miss.

---

## 👥 6. Identifying Stakeholders

### Stakeholder Impact Analysis

| Stakeholder | Problem They Face | Solution Benefit |
|-------------|------------------|------------------|
| **👤 Customers** | Service issues, poor experience | Service improvements & targeted support |
| **🏪 Sellers** | Platform instability, low visibility | Stable tools & increased item selection chances |
| **💰 Investors** | Unsustainable growth metrics | Profit & sustainable business model |
| **👨‍💼 Employees** | Manual, guesswork-based decisions | Increased productivity & data-driven analysis |
| **👔 Founder** | Revenue decline, market competition | High revenue, competitive advantage, customer insights |

---

## 🤖 7. Define the AI Task - ML Formulation

### Problem Type: Multi-Task Approach

| Task | Description | Use Case |
|------|-------------|----------|
| **🏷️ Classification** | Predict 'Stay' or 'Leave' | Identify who will churn |
| **👥 Segmentation** | Cluster customers by behavior | Tailor retention strategies |
| **⚠️ Risk Scoring** | Score probability of churn | Prioritize intervention efforts |

### Suggested ML Models

| Model | Purpose | Pros | Cons |
|-------|---------|------|------|
| **Logistic Regression** | Baseline classification | Simple, interpretable | May underfit complex patterns |
| **Random Forest** | Feature importance analysis | Handles non-linearity, robust | Less interpretable |
| **XGBoost** | High performance prediction | State-of-the-art accuracy | Requires careful tuning |
| **K-Means Clustering** | Customer segmentation | Scalable, easy to implement | Requires feature scaling |

### 🎯 Recommended Pipeline
1. Start with **Logistic Regression** (baseline)
2. Use **Random Forest** for feature importance
3. Deploy **XGBoost** for production (best performance)
4. Apply **K-Means** for customer segmentation

---

## 📊 8. Determining Success Metrics

### Classification Metrics

| Metric | Definition | Why It Matters |
|--------|-----------|-----------------|
| **📈 Accuracy** | Correct predictions / Total predictions | Overall model performance |
| **🎯 Precision** | True positives / (TP + FP) | Avoid false alarms (wasted offers) |
| **🔍 Recall** | True positives / (TP + FN) | **MOST IMPORTANT** - Don't miss churners |
| **⚖️ F1 Score** | Harmonic mean of precision & recall | Balanced performance metric |

### 🏆 Priority Metric: **RECALL**

**Why Recall is Most Important:**
- ✅ We want to catch **as many at-risk customers as possible**
- ✅ Missing a churning customer is more costly than false positives
- ✅ Cost of retention offer << Cost of losing a customer
- ✅ Better to over-predict churn than under-predict

### 💼 Business Metrics
- 📉 Overall churn rate reduction: **Target 8-10%**
- 💰 Customer retention cost vs. acquisition cost
- 📊 Customer lifetime value improvement
- ⏰ Time to implement retention actions

---

## ⚙️ 9. Defining Constraints

### 🏢 Operational Constraints
- 💵 Limited budget for retention discounts/offers
- ⏱️ Limited time to implement interventions
- 👥 Limited customer service capacity for personalized outreach

### 📂 Data Constraints
- ❌ Missing financial records for some transactions
- ❌ Customer preferences change over time (hard to capture)
- ❌ Limited historical data for newly acquired customers
- ❌ Last 3 months data may have quality issues (system migration)

### 🔒 Ethical Constraints
- 🛡️ Protection of customer personal data
- ⚖️ Non-manipulation (avoid deceptive offers)
- 📋 Compliance with data privacy regulations (GDPR, etc.)
- 🚫 Fair treatment across customer segments

---

## 🚨 10. Determining Assumptions and Risks

### ✅ Key Assumptions

| Assumption | Description | Validation Plan |
|-----------|-------------|-----------------|
| **Historic data is predictive** | Past behavior predicts future churn | Validate with holdout test set |
| **60-day rule** | 60-day inactivity = churned customer | Confirm with business stakeholders |
| **Actions will be executed** | Retention strategies will be implemented | Management commitment |
| **Model generalization** | Patterns hold across all segments | Test across demographic segments |

### ⚠️ Known Risks

| Risk | Impact | Mitigation |
|------|--------|-----------|
| **Missing Data** | Reduced model accuracy | Imputation strategy + sensitivity analysis |
| **Data Bias** | Model inherits historical biases | Audit for bias across demographics |
| **Poor Generalization** | Works for some segments, not others | Cross-segment validation |
| **Limited Labeled Data** | Insufficient validation samples | Use stratified sampling + resampling |
| **Model Drift** | Performance degrades over time | Regular retraining & monitoring |

---

## 🎯 Implementation Roadmap

### Phase 1: Data & Exploration
- [ ] Collect historical customer data
- [ ] Exploratory Data Analysis (EDA)
- [ ] Feature engineering & selection

### Phase 2: Modeling
- [ ] Baseline model (Logistic Regression)
- [ ] Advanced models (XGBoost, Random Forest)
- [ ] Hyperparameter tuning
- [ ] Model evaluation & comparison

### Phase 3: Segmentation & Strategy
- [ ] Customer segmentation (K-Means)
- [ ] Define retention strategies per segment
- [ ] Estimate ROI of interventions

### Phase 4: Deployment & Monitoring
- [ ] Model deployment to production
- [ ] Implement retention actions
- [ ] Track performance metrics
- [ ] Regular retraining pipeline

---

## 📝 Summary

This problem scoping document establishes the foundation for a **data-driven churn prediction project** that will:

✅ Identify at-risk customers before they leave  
✅ Enable targeted retention strategies  
✅ Reduce churn rate by 8-10%  
✅ Improve customer lifetime value  
✅ Provide competitive advantage  

**Next Step:** Begin data collection and exploratory analysis phase.

---

*Last Updated: 2026-06-17*
