
Title: Data Quality, Uncertainty, and Conservatism
Published: September 2026 

# Data Quality and Uncertainty
Data quality and uncertainty are related, but they are not direct opposites. Data quality describes whether information is accurate, complete, representative, and suitable for its intended use. Uncertainty describes the limits of what can be concluded from that information.

High-quality data can still carry substantial uncertainty. A geotechnical sample may be accurately measured (e.g., a Cone Penetration Test (CPT)) but provide little evidence of conditions between widely spaced locations; in the same sense, the data measurement at a single depth interval can be precise but inaccurate. Where several datasets are combined, uncertainty can compound through differences in resolution, coverage, survey age, interpretation, and underlying assumptions. For complex and multi-stage analyses, uncertainty is particularly important to understand and assess.

## Identifying Uncertainty
Uncertainty should be assessed in relation to the decision being made. For example, data suitable for concept route selection may not be adequate for detailed burial design.

Common sources include:
- Sparse or uneven data coverage
- Measurement and positioning error
- Limited geophysical resolution or penetration
- Extrapolation between sampled locations
- Interpretation of indirect evidence
- Spatial and temporal variability
- Conflicting evidence between datasets
- Simplifying assumptions within the model

The source and engineering consequence of each uncertainty should be recorded. A high, medium, or low rating is most useful when supported by a clear explanation. This grading system is universally understood and simple to convey to any audience, technical or non-technical.

## Assessing and Modelling Uncertainty
Data quality and uncertainty should be graded separately. A high-quality point measurement may still have high spatial uncertainty if it is used to represent a large or variable area. The applied method to assess uncertainty should reflect the available evidence and the importance of the decision.

Uncertainty can be assessed using:
- Sensitivity analysis
- Parameter ranges
- Low, best, and high estimates
- Geostatistical interpolation
- Probability distributions
- Bayesian analysis
- Monte Carlo simulations

## Low, Best, and High Estimates
Low, best, and high estimates provide a practical way to test how uncertain inputs affect an engineering conclusion.

- **Low estimate:** A credible lower-bound value, not simply the most favourable case
- **Best estimate:** The most likely or best-supported value
- **High estimate:** A credible upper-bound value, not exactly the worst case scenario

Low-estimate (LE), best-estimate (BE), and high-estimate (HE) soil profiles are commonly used to assess jack-up leg penetration, punch-through, and recovery. If the LE and HE profiles produce substantially different outcomes, such as shallow penetration under one case and deep penetration or punch-through under another, the ground model may be too uncertain to support a reliable decision. Further geotechnical sampling could then be justified, because the cost and delay are minor compared with the potential consequences of severe punch-through or vessel instability. 

This approach is transparent and proportionate where the data or project budget do not justify a full probabilistic model. It also shows whether the design is sensitive to an uncertain parameter or remains broadly unchanged across the reasonable range.

## Uncertainty in Offshore Cable Engineering
In a Cable Burial Risk Assessment (CBRA), uncertainty is commonly evaluated using the quality, coverage, and agreement of geophysical, geotechnical, environmental, and vessel activity data.

For example, shallow biogenic gas may cause acoustic blanking in sub-bottom profiler data, preventing interpretation of the underlying geology, particularly where geotechnical sampling could not be conducted due to the weak soil strength. The affected section should be identified as uncertain rather than assigned a definitive ground classification; there could be an underlying hard layer that is not visible in the assessment, or there could be 10s of meters of weak material.

Other common sources include:
- Widely spaced geotechnical samples
- Limited sampling of the mobile surficial layer
- Sparse particle size distribution data
- Uncertain correlation between geophysical units and geotechnically sampled material
- Poor quality geophysical interpretation
- Reliance on regional seabed classifications
- Changes in seabed level or bedform position between surveys

These uncertainties should be linked to their possible consequences to aid route engineering and carried through to the Burial Assessment Study (BAS), informing tool selection, achievable burial depth, installation rate, cable protection recommendations, and residual risk.

## Kriging and Monte Carlo Simulations
Statistical quantitative methods can be applied to extend sampled datasets, model multiple scenarios, and present uncertainty; however, their limitations should be carefully considered before and during implementation.

### Kriging
Kriging estimates values between sampled locations using observed spatial relationships. It can also provide an estimate of interpolation uncertainty. 

Kriging cannot identify a geological feature that is absent from the input data (unknowns). For example, Particle Size Distribution (PSD) data at KP5 and KP6 may indicate medium sand, while geophysical data between the locations identify a gravel patch and dense boulder field. Interpolating only the available PSD data points would smooth across this coarse feature and misrepresent the ground conditions.

A better approach is to integrate the data and treat the gravel and boulder area as a separate geological zone. It may be assigned a representative grain-size range using comparable nearby samples, regional evidence, or a documented engineering assumption. The value must remain clearly identified as inferred and uncertain, rather than measured.

### Monte Carlo Simulations
Monte Carlo simulation tests how uncertain inputs affect the range and probability of modelled outcomes. Instead of using one fixed value for each parameter, values are sampled repeatedly from defined probability distributions.

Applications for CBRAs may include uncertainty in:
- Grain size and soil strengths
- Layer thicknesses
- Probability parameters (engine loss, anchor deployment, vessel activity, etc.)
- Anchor embedment depths
- Achievable burial depths

The result is a distribution of possible outcomes rather than a single deterministic value. This can identify the probability of meeting a burial requirement and the parameters that control the result.

Monte Carlo simulation should not be treated as a substitute for an exhaustive grid search. Its main purpose is to propagate uncertainty through the analysis. For example, highly uncertain areas may be marked for further sampling or re-routeing.

## Conservatism and Overly Conservative Models
Conservatism is necessary where evidence is incomplete or failure has serious consequences. However, adding conservative assumptions independently at each stage of a CBRA or BAS can create a compounded result that is no longer proportionate to the underlying risk.

For example, conservative assumptions may be applied to the same uncertainty parameters in the previous section, particularly probability of engine failure and anchor embedment depths within CBRAs. When this is paired with a conservative Vertical Reference Level (VRL) - defining a level where the CBRA's depth should begin to mitigate seabed mobility hazards - the combined conservative assumptions result in a Depth of Lowering (DoL) that may be difficult or impossible to achieve. The concern is therefore primarily how conservatism is combined and applied across the CBRA and BAS process on a system-level scale.

Excessive burial can introduce other engineering constraints:
- Tool depth and operational limits
- Reduced effectiveness or increased risk from additional passes
- Cable thermal derating at greater burial depths
- Increased installation cost and programme risk
- More difficult cable repair, recovery, or replacement if parts become defective
- Greater dependence on uncertain predictions of tool performance

A defensible design should consider burial risk, installation feasibility, cable thermal performance, and recoverability together. Where the assessed DoL is not practicable, the response should not automatically be a more powerful burial tool or repeated passes. Route adjustment, alternative protection, acceptance of residual risk, or changes to the design basis may provide a better whole-life solution.

## Integrating Sparse and Regional Data
Sparse geotechnical samples are often combined with geophysical interpretation and regional mapping. This improves spatial coverage but can introduce uncertainty because the datasets represent different scales and types of evidence.

A defensible integrated cable study should:
- Separate measured, interpreted, and inferred values
- Divide the route into meaningful geological zones for the assessment purpose
- Record the evidence supporting each zone
- Grade uncertainty according to data density and agreement
- Test credible low, best, and high estimates
- Identify where additional investigation could change the design (and reduce uncertainty)

The purpose is to show how uncertainty affects the engineering decision, while preventing concealment of weak evidence.
