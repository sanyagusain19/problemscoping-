# E-Commerce Churn Rate Problem Scoping

## 📌 Project Overview

This repository contains comprehensive **problem framing and scoping documentation** for an **AI/ML project aimed at predicting and reducing customer churn rate** in an e-commerce platform.

**Current Challenge:** A sharp increase in churn rate from 28% → 38% over the past 6 months, representing a critical business problem requiring data-driven investigation and intervention.

---

## 🎯 Key Objectives

- **Identify** customers at risk of churning
- **Predict** churn probability using machine learning
- **Segment** customers for targeted retention strategies
- **Reduce** overall churn rate by 8-10% through proactive interventions

---

## 📊 Business Impact

- **Acquisition Cost:** New customers cost 5x more to acquire than retaining existing ones
- **Revenue Threat:** High churn directly impacts Customer Lifetime Value (CLV)
- **Competitive Risk:** In a crowded market, churn signals unsustainable growth to investors

---

## 📂 Repository Contents

- **`problem_scoping_churn_rate.md`** — Complete problem framing document covering:
  - Problem discovery and timeline
  - Stakeholder perspectives (technical, management, business)
  - Business justification and impact
  - AI/ML approach and model selection
  - Success metrics and constraints
  - Assumptions and risks

---

## 🔍 Problem Scoping Breakdown

### 1. **Problem Identification**
- Current churn rate: 28-30% (increased to 38% over 6 months)
- Suspected causes: Payment gateway update, UI redesign, delivery partner change, reduced discounts

### 2. **Stakeholder Analysis**
- **Customers:** Problem resolution and service improvement
- **Sellers:** Stable platform and increased visibility
- **Investors:** Profit and sustainable growth metrics
- **Employees & Management:** Enhanced productivity through data-driven insights

### 3. **AI/ML Formulation**
- **Task Type:** Classification + Segmentation + Risk Scoring
- **Suggested Models:**
  - Logistic Regression (baseline)
  - Random Forest (feature importance)
  - XGBoost (high performance)
  - K-Means Clustering (segmentation)

### 4. **Success Metrics**
- **Primary:** Recall (catch as many at-risk customers as possible)
- **Secondary:** Precision, F1 Score, Accuracy
- **Business Metric:** 8-10% reduction in overall churn rate

### 5. **Key Constraints**
- **Operational:** Limited budget for discounts/retention offers
- **Data:** Quality issues, missing historical data for new customers, incomplete financial records
- **Ethical:** Customer privacy protection, avoid manipulation

---

## 🚀 Next Steps

1. **Data Collection & EDA** — Gather historical customer data and explore patterns
2. **Feature Engineering** — Create predictive features (recency, frequency, engagement, etc.)
3. **Model Development** — Build and compare baseline and advanced models
4. **Customer Segmentation** — Identify high-risk customer groups
5. **Retention Strategy** — Design targeted interventions (discounts, offers, support)
6. **Deployment & Monitoring** — Deploy model and track performance over time

---

## 📋 Key Assumptions

- Historic data is indicative of future customer behavior
- 60-day inactivity = churned customer (to be validated)
- Retention actions will be executed according to customer segments
- Model patterns will generalize across customer segments

---

## ⚠️ Known Risks

- Missing or incomplete data
- Bias in historical data
- Model may not generalize well across all segments
- Limited labeled data for validation

---

## 👥 Stakeholders

| Stakeholder | Interest | Impact |
|------------|----------|--------|
| **Customers** | Better service & problem resolution | Improved experience |
| **Sellers** | Platform stability & visibility | Increased sales |
| **Investors** | Sustainable growth & profitability | Confidence in business |
| **Management** | Data-driven decision making | Reduced guesswork |
| **Founder** | Revenue growth & competitive advantage | Market leadership |

---

## 📖 How to Use This Repository

1. Start with **`problem_scoping_churn_rate.md`** for detailed problem analysis
2. Use this README as a quick reference guide
3. Future phases will include: exploratory notebooks, data pipelines, model implementations
4. Track progress through GitHub Issues

---

## 🏷️ Topics

`machine-learning` | `churn-prediction` | `e-commerce` | `data-science` | `problem-scoping`
