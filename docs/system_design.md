System Design – Project 2

The proposed system integrates machine learning-based defect risk prediction with test case prioritization.

Static code metrics are first used to train a defect prediction model, which produces risk scores for software modules. These risk scores are then utilized to prioritize test cases based on the modules they cover. Test cases associated with higher-risk modules are executed earlier to improve fault detection effectiveness under limited testing time.

The approach is evaluated by comparing risk-based prioritization against baseline strategies such as random and original test execution orders.


Simulated Test Case Mapping

To enable test case prioritization, a simulated test–module coverage mapping was generated. Each test case was randomly associated with one to three software modules using a fixed random seed to ensure reproducibility. This approach reflects common research practice when real test coverage information is unavailable.

Test Risk Score Computation

Defect risk scores predicted at the module level are propagated to test cases using a summation-based aggregation strategy. Each test case’s risk score is computed as the sum of defect probabilities of the modules it covers. Test cases are then prioritized in descending order of computed risk scores.

