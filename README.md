# Optimizing LRPC Strand Production at Usha Martin: A Strategic Application of PERT/CPM Analysis.

![Project Status](https://img.shields.io/badge/Status-Complete-success)

## 1. Executive Summary

This report presents a comprehensive analysis of the Low Relaxation Prestressed Concrete (LRPC) strand production process at Usha Martin.It applies a synthesized Program Evaluation and Review Technique (PERT) and Critical Path Method (CPM) framework to model the manufacturing workflow, quantify schedule risks, and provide actionable recommendations for process optimization.

The analysis identifies the critical path of production, calculates a total expected production duration of **71.34 hours**, and quantifies the schedule risk, providing a path for Usha Martin to enhance production predictability and maintain its competitive advantage.
<p align="center">
<img width="634" height="266" alt="CPM DIAGRAM DRAW IO" src="https://github.com/user-attachments/assets/4e2b17ed-f8f3-4054-90ae-ce2154a4df09" />
</p>

## 2. Project Objectives

The primary objectives of this analysis were to:

* Model the complex, interdependent manufacturing workflow of LRPC strands.
* Identify operational bottlenecks that constrain the plant's throughput.
* Quantify schedule risks using probabilistic methods.
* Provide data-driven, actionable recommendations for process optimization and resource allocation.

---

## 3. Methodology: A Hybrid PERT/CPM Framework

This project integrates the strengths of two established project management techniques.

### Program Evaluation and Review Technique (PERT)

PERT's probabilistic approach was used to handle the uncertainty and variability inherent in manufacturing. By using a three-point time estimate for each activity, a statistically robust **Expected Time (ET)** was calculated.

* **Optimistic Time (O):** The minimum possible time.
* **Most Likely Time (M):** The most realistic time under normal conditions.
* **Pessimistic Time (P):** The maximum possible time, assuming delays.

The weighted average formula used is:
$$ET = \frac{O + 4M + P}{6}$$

### Critical Path Method (CPM)

CPM's deterministic algorithm provided the scheduling framework. It was used to:
* Identify the **Critical Path**: The longest sequence of dependent tasks that determines the total project duration. Activities on this path have zero "float" or "slack".
* Calculate **Total Float (TF)**: The amount of time a non-critical activity can be delayed without affecting the project's final completion date.

$$TF = LS - ES \quad \text{or} \quad TF = LF - EF$$

---

## 4. The Case Study: LRPC Production Workflow

The analysis decomposed the entire production run into a granular Work Breakdown Structure (WBS).

### Work Breakdown Structure (WBS) and Dependencies

| Activity ID | Activity Description | Immediate Predecessor(s) |
| :--- | :--- | :--- |
| **A** | Raw Material Intake & Inspection | - |
| **B** | Surface Treatment/Descaling | A |
| **C** | Production Line Setup & Calibration | B |
| **D** | First Drawing | C |
| **E** | Patenting (Heat Treatment) | D |
| **F** | Intermediate Drawing | E |
| **G** | Stranding | F |
| **H** | Thermal Treatment (Stabilization) | G |
| **I** | Closing/Finishing | H |
| **J** | In-House QA Testing (Batch Sample) | H |
| **K** | Final Packaging & Labeling | I, J |
| **L** | Preparation for Dispatch | K |

---

## 5. Core Analysis & Key Findings

The CPM algorithm was applied to the WBS using the Expected Times (ET) calculated from PERT estimates. The full calculation matrix below synthesizes the results.

### Critical Path Method (CPM) Calculation Matrix (Durations in Hours)

| ID | Duration (ET) | ES | EF | LS | LF | Total Float (TF) | On Critical Path? |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **A** | 6.33 | 0.00 | 6.33 | 0.00 | 6.33 | **0.00** | **Yes** |
| **B** | 1.17 | 6.33 | 7.50 | 6.33 | 7.50 | **0.00** | **Yes** |
| **C** | 4.50 | 7.50 | 12.00 | 7.50 | 12.00 | **0.00** | **Yes** |
| **D** | 2.67 | 12.00 | 14.67 | 12.00 | 14.67 | **0.00** | **Yes** |
| **E** | 8.17 | 14.67 | 22.84 | 14.67 | 22.84 | **0.00** | **Yes** |
| **F** | 4.17 | 22.84 | 27.01 | 22.84 | 27.01 | **0.00** | **Yes** |
| **G** | 10.33 | 27.01 | 37.34 | 27.01 | 37.34 | **0.00** | **Yes** |
| **H** | 17.00 | 37.34 | 54.34 | 37.34 | 54.34 | **0.00** | **Yes** |
| **I** | 3.00 | 54.34 | 57.34 | 62.34 | 65.34 | **8.00** | No |
| **J** | 11.00 | 54.34 | 65.34 | 54.34 | 65.34 | **0.00** | **Yes** |
| **K** | 4.00 | 65.34 | 69.34 | 65.34 | 69.34 | **0.00** | **Yes** |
| **L** | 2.00 | 69.34 | **71.34** | 69.34 | **71.34** | **0.00** | **Yes** |

### Summary of Findings

1.  **Total Project Duration:** The total expected time for a single production run is **71.34 hours**.
2.  **Critical Path Identified:** The critical path is the sequence of 11 activities with zero float:
    **$A \rightarrow B \rightarrow C \rightarrow D \rightarrow E \rightarrow F \rightarrow G \rightarrow H \rightarrow J \rightarrow K \rightarrow L$**.
3.  **Production Bottlenecks:** These critical path activities—from raw material intake through QA testing—are the primary constraints on the plant's throughput. Any delay in these tasks will directly delay the final dispatch.
4.  **Non-Critical Activity:** Activity **I (Closing/Finishing)** is the only non-critical activity, with a **Total Float of 8.00 hours**This means the finishing process can be delayed by up to 8 hours without impacting the final deadline.

---

## 6. Strategic Recommendations

The analysis yields several actionable directives for management:

### 1. Focus Improvement on the Critical Path

To shorten the 71.34-hour production cycle, continuous improvement initiatives (like Kaizen or Six Sigma) and capital investment must be concentrated on the 11 critical path activities. Optimizing the non-critical Activity I will not reduce the total production time.

### 2. Quantify and Manage Schedule Risk

The project's overall standard deviation ($\sigma_P$) was calculated to be **3.03 hours**.This metric moves risk management from a qualitative guess to a data-driven discipline, allowing for probabilistic forecasting:

* There is a **~68% probability** of completing the run between **68.31 and 74.37 hours**.
* There is a **~95% probability** of completing the run between **65.28 and 77.40 hours**.

This data enables the sales team to provide customers with credible, data-backed delivery windows, building trust and managing expectations.

### 3. Leverage "Float" for Efficiency

The **8.00 hours of float** on Activity I (Closing/Finishing) is a valuable operational resource. This flexibility can be strategically managed to:
* **Level Resources:** Temporarily re-deploy personnel from finishing to assist a delayed critical path activity.
* **Save Costs:** Schedule the finishing task during off-peak hours to take advantage of lower electricity tariffs.
* **Schedule Maintenance:** Perform preventative maintenance on finishing equipment within this 8-hour window without halting the entire line.

### 4. Accelerate Schedules Logically

When faced with urgent orders, the analysis provides a clear framework for schedule compression:
* **Crashing:** Allocating additional resources (e.g., overtime, extra machinery) should *only* be applied to critical path activities like "Thermal Treatment" (H) or "Stranding" .
* **Fast-Tracking:** Re-engineering the process to run critical tasks in parallel (e.g., starting preliminary QA tests before all of "Thermal Treatment" is complete) can save time but must be managed for increased risk.

## 7. Conclusion

The integration of PERT and CPM provides Usha Martin with a dynamic and predictive model to optimize its LRPC production. By identifying the critical path, quantifying schedule risk , and strategically managing float , the company can significantly enhance production predictability, improve resource efficiency, and solidify its competitive advantage as a reliable, "one-stop solution provider".
