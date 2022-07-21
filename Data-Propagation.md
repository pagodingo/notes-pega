# Propagating data from one case to another

## Propagation through Data Transforms & Automation Shapes

*Child-to-Parent Data Propagation:*

1. **Create Parent Case**
     - <u>2  Stages</u>
          - Stage (New)
               - Step: New (Blank)
               - Step: Create child case (Automation)
               - Step: Wait (Automation): **condition**: *until child case(s) resolve*
          - Stage (Display child case: data)
               - Step: Display Child Data
                    - 1 field: Data from child -- type: text(single line) --
2. **Create Child Case**
     - <u>1  Stage</u>
          - Stage (New)
               - Step: Data (Collect info) -- Set Case Status to *Resolved-Completed*
                    - 1 field: _Data_ --Type: text (single line)
               - Step: Update Case (Automation)
               > ensures parent case is refreshed and new data is shown
3. Configure child case > Open Process > Configure **Update Case**

<img src="./images/childtoparent-updatecase.png" />
<img src="./images/childtoparent-datatransform.png" />
<img src="./images/childtoparent-referencedpages.png" />

---

**Run:**

<img src="./images/childtoparent-1.png" />
<img src="./images/childtoparent-2.png" />
<img src="./images/childtoparent-3.png" />
<img src="./images/childtoparent-4.png" />
<img src="./images/childtoparent-5.png" />
<img src="./images/childtoparent-6.png" />
