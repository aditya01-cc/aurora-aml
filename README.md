Aurora: Autonomous AML Intelligence
Detect. Explain. Narrate. Locally.

Aurora is a conceptual and technical demonstration of a real-time fraud early warning system designed for the Australian financial landscape. It is built to resolve the "Productivity Paradox" in finance by redesigning decision architecture around the complementary strengths of human judgment and machine intelligence.
1. The Core Problem

Australian financial institutions face a significant challenge: record technology spending in early 2025 has not yet lowered cost-to-income ratios, which rose 89 basis points to 49.2%. Meanwhile, fraud losses reached AUD 2.74 billion across the economy in 2023–24. Aurora addresses these gaps by moving beyond supervised models trained on historical data, which often fail to detect novel, adversarial fraud patterns.
2. Architectural Pillars

Aurora is built on an architectural philosophy of signal synthesis rather than simple pattern matching:

    Real-Time Feature Engineering: Features are computed from raw event streams at the moment of transaction, capturing emerging behavioral signatures that batch-processed systems miss.

    Ensemble Independence: The system combines independent model architectures—including XGBoost on structured features and an Isolation Forest on behavioral sequences—fused through a calibrated meta-learner.

    SHAP-Grounded Explainability: Every prediction is decomposed into additive feature contributions using SHAP (SHapley Additive exPlanations) values. This ensures that model reasoning is transparent and auditable.

    Narrative Synthesis Layer: A Large Language Model (LLM) translates quantitative SHAP decompositions into decision-quality narratives. This layer acts as a synthesis and narration tool, not a reasoning layer, ensuring all output is grounded in structured input.

3. AUSTRAC Typologies & Signals

Aurora is engineered to detect behavioral signals consistent with AUSTRAC transaction monitoring obligations:
Signal	Rationale
Transaction Velocity	

Identifies account takeover and card testing attacks via rolling 1-minute to 1-hour windows.
Geographic Velocity	

Detects impossible location transitions consistent with card-not-present fraud.
Temporal Anomaly	

Flags transactions occurring at unusual hours, a common sign of scam-induced activity.
Session Age	

Captures the characteristic duration of Authorized Push Payment (APP) scam sessions.
Peer Deviation	

Identifies transactions that are anomalous relative to a customer’s peer group (age, income, tenure).
4. Governance & Regulatory Alignment

Aurora is designed to meet rigorous Australian regulatory expectations:

    APRA CPS 230: Supports operational risk management through documented model inventory and clear human accountability for material decisions.

    ASIC Guardrail 7: Provides the transparency required for AI safety standards through SHAP-based interpretability.

    AUSTRAC Alignment: Generates structured evidence chains that map directly to the "grounds for suspicion" required for suspicious matter reports.

5. Performance Benchmarks
Metric	Target	Rationale
AUPRC	> 0.72	

Reflects true precision-recall trade-off on imbalanced fraud datasets.
SHAP Coverage	> 85%	

Ensures explanations are concise and operationally useful for analysts.
Latency	< 800ms	

Required for scoring within the standard transaction authorization window.
6. A Note on the Project’s Origins

Aurora is the result of a personal deep-dive into the future of financial intelligence. This project was conceived and built entirely as an independent research initiative, born from an after-hours curiosity about how we can better protect the Australian financial ecosystem.

    Personal Research: This work represents my own independent analysis and does not reflect the official position of any institution or employer.

    Independent Development: Aurora was developed using personally owned resources and personal time.

    Data Integrity: To prioritize privacy and security, all data used in this technical demonstration is synthetic.

I view this project as a personal contribution to the global conversation on AI transparency and human-machine partnership. It is an independent labor of love, created to explore the art of the possible in a rapidly evolving world.
Reference

This technical demonstration supports the working paper:

Roy, A. (2026). The Intelligent Finance Function: Why the Future of Financial Decision-Making Is Human, Machine, and Something New Entirely.
