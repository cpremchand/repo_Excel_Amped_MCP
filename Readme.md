# Test Case Excel Generation from SRS

## Objective
Generate a comprehensive Excel file for **Validation Testing** and **Integration Testing** based on your SRS (Software Requirements Specification) document.  
Each functional and non-functional requirement from the SRS will be mapped to one or more test cases, including edge cases.

---

## Instructions

1. **Input**:  
   Provide your SRS document.

2. **Test Case Coverage**:  
   - For **every** functional and non-functional requirement, create multiple test cases as needed to cover all normal, boundary, and edge scenarios.
   - Cover both **Validation Testing** and **Integration Testing**.

3. **Excel Output**:  
   - Save the file as: `test_cases.xlsx`  
   - Path: `D:\archive\test_hub\test_now\AI_POC_Ideas\repo_Excel_Amped_MCP`
   - Sheet name: `test_cases`

4. **Excel Columns**:  
   | Traceability Req-ID | Test Case ID | Priority | Test Case Objective | Test Precondition | Test Steps | Test Inputs (Conditions / Values) | Test Case Design Methodology | Dependent Test Cases | Expected Outcome |

---

## Example Row

| Traceability Req-ID | Test Case ID | Priority | Test Case Objective | Test Precondition | Test Steps | Test Inputs (Conditions / Values) | Test Case Design Methodology | Dependent Test Cases | Expected Outcome |
|---------------------|--------------|----------|---------------------|-------------------|------------|-----------------------------------|-----------------------------|----------------------|------------------|
| FR1.1 | TC_VD_001 | P1 | Verify that the system detects vehicle presence using IR sensor on GPIO P0.7 | System initialized, IR sensor connected to P0.7, no vehicle present initially | 1. Power on the system 2. Place a vehicle in front of IR sensor 3. Observe system response 4. Remove vehicle | Vehicle presence simulation at IR sensor | Black Box Testing | None | System detects vehicle and initiates transaction processing |

---

## Few-Shot Prompt to Use

```
You are given an SRS (Software Requirements Specification) document. Using this document, generate an Excel file for both Validation Testing and Integration Testing and Unit Testing. For each functional and non-functional requirement in the SRS, create all applicable test cases, including edge cases. Each requirement may have multiple test cases.

Format each row in the Excel as follows (see example):

| Traceability Req-ID | Test Case ID | Priority | Test Case Objective | Test Precondition | Test Steps | Test Inputs (Conditions / Values) | Test Case Design Methodology | Dependent Test Cases | Expected Outcome |

Example Row:
| FR1.1 | TC_VD_001 | P1 | Verify that the system detects vehicle presence using IR sensor on GPIO P0.7 | System initialized, IR sensor connected to P0.7, no vehicle present initially | 1. Power on the system 2. Place a vehicle in front of IR sensor 3. Observe system response 4. Remove vehicle | Vehicle presence simulation at IR sensor | Black Box Testing | None | System detects vehicle and initiates transaction processing |

Instructions:
- For every requirement (functional and non-functional), generate as many test cases as needed to cover all normal, boundary, and edge scenarios.
- Include both Validation Testing and Integration Testing and Unit Testing test cases.
- Use clear, concise language and ensure traceability to the SRS requirements.
- Save the resulting Excel file as test_cases.xlsx in the path: D:\archive\test_hub\test_now\AI_POC_Ideas\repo_Excel_Amped_MCP.
- Sheet name: test_cases.

Columns to include:
- Traceability Req-ID
- Test Case ID
- Priority
- Test Case Objective
- Test Precondition
- Test Steps
- Test Inputs (Conditions / Values)
- Test Case Design Methodology
- Dependent Test Cases
- Expected Outcome

Use the SRS document provided to populate the test cases as per the above template and instructions.
```

---
