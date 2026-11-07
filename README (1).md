# **4PM STREET**

## **Shadow \+ Heat Memory**

**Thermal Commons \| A3 — Grounded Instrument**

### **Project Description**

4PM STREET is an interactive architectural design instrument that investigates the relationship between solar movement, shade placement, and pavement heat retention along an urban pedestrian route in Austin, Texas.

The project emerged from an investigation of afternoon thermal exposure and the potential of environmental measurements to inform architectural design decisions.

Rather than treating shade as a fixed area of coverage, the instrument examines shade as a changing spatial and temporal condition. Trees and canopies cast moving shadows, while pavement retains heat from earlier exposure. The resulting pattern reveals where thermal discontinuities persist along the walking route.

The central design question is:

**Can strategically distributed shade reduce the longest overheated gap along a pedestrian route more effectively than concentrated shade under the same intervention budget?**

### **How the Instrument Works**

Users can add and reposition trees and canopies within a 114-meter pedestrian route. The instrument simulates afternoon solar movement from 12 PM to 5 PM and calculates a simplified estimate of surface temperature and accumulated sun exposure.

The interface provides three visual modes:

* **Current Shadow:** The location and extent of shadows at a selected time.  
* **Cumulative Exposure:** Accumulated exposure throughout the afternoon.  
* **Surface Heat:** Estimated pavement temperatures based on heating, cooling, and thermal storage assumptions.

Outputs include exposure minutes, peak surface temperature, cool-route percentage, shade budget, and longest hot gap.

A rule-based proposal system evaluates design changes and can refuse configurations that fail its constraints. Users can revise their proposals and record successive rounds.

### **A3 Grounding Tools**

**1\. Physics Check**

The instrument verifies shadow geometry using the established relationship:

L \= h / tan(α)

where L is shadow length, h is object height, and α is solar altitude.

The test compares theoretical and simulated shadow lengths and reports numerical deviations.

**2\. Temperature Data Input**

The application accepts temperature observations with associated dates, times, materials, and sun/shade conditions. Measurements can be entered manually or imported from CSV files.

**3\. Cooling-Curve Calibration**

The application fits an exponential cooling relationship to a temperature series. The resulting cooling parameter can be applied to the thermal simulation.

These tools distinguish geometric verification from empirical thermal calibration.

### **How to Use**

1. Open the application in a desktop browser.  
2. Select the simulation date.  
3. Place or move trees and canopies along the route.  
4. Run the afternoon simulation.  
5. Review the surface heat and longest-hot-gap outputs.  
6. Use the Physics Check to inspect shadow geometry.  
7. Import a documented dataset into the appropriate calibration tool.  
8. Evaluate the fitted cooling model and its limitations.  
9. Revise the design and compare the resulting outputs.

### **Research Basis**

The instrument draws on established solar geometry and published research on urban shade, pavement temperatures, and thermal behavior.

Reference sources include:

* NOAA Global Monitoring Laboratory, *General Solar Position Calculations*.  
* Middel et al., *50 Grades of Shade* (2021).  
* Published experimental research on the thermal behavior of shaded and unshaded pavement.

Published research provides external reference evidence. Data taken from research publications must retain the original source, measurement context, units, and observation status.

### **Known Limitations**

4PM STREET is a simplified architectural design instrument, not a fully validated microclimate model.

The model idealizes tree geometry, canopy form, pavement properties, and environmental conditions. It does not comprehensively simulate wind, humidity, evapotranspiration, or human thermal comfort.

Predicted surface temperatures depend on adjustable assumptions and calibration inputs. A successful geometric verification does not establish thermal prediction accuracy.

Research measurements collected in other locations may not directly represent Austin's climate, pavement materials, or site conditions.

### **Development Process**

The project developed through three stages:

**A1 — Thermal Commons:** Investigating thermal exposure as an architectural design layer.

**A2 — Interactive Playground:** Testing moving shade, heat memory, and the longest continuous hot gap.

**A3 — Grounding Instrument:** Introducing numerical geometry verification, empirical data handling, and cooling-model calibration.

The application was developed with AI-assisted programming using Claude and browser-based HTML, CSS, and JavaScript.

### **Project Status**

A3 Stage 1 implementation. The numerical geometry check and calibration interface are implemented; independent thermal validation and final comparative testing require documented evidence.

