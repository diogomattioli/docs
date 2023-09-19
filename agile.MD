## Story Points

| Story Points | Effort and Complexity Definition                                           | Example Tasks                                                                                                              | Level of Uncertainty                 | Uncertainty Legend                              |
|--------------|-----------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|-------------------------------------|-------------------------------------------------|
| 0            | No effort is required. Task is trivial and can be completed instantly.    | Updating a comment in the code.                                                                                           | Very Low                            | Task outcome is almost certain.                |
| 1            | Minimal effort. Task is straightforward with very little complexity.      | Adding a simple configuration parameter to the backend.                                                                  | Low                                 | Minimal chance of unexpected challenges.       |
| 2            | Low effort. Task is simple, might have minor complexities or dependencies.| Implementing a basic error handling mechanism in the hardware communication layer.                                      | Low                                 | Some potential challenges but manageable.     |
| 3            | Moderate effort. Task is of moderate complexity with some challenges.     | Integrating a new hardware device with an existing driver and creating a basic API endpoint for it.                     | Moderate                            | Moderate uncertainty; expect some surprises.  |
| 5            | Moderate to high effort. Some complexities, minor risks or uncertainty.   | Developing a new feature that requires optimizing the communication protocol between the embedded system and backend.    | Moderate                            | Fair amount of uncertainty and potential risks. |
| 8            | High effort. Task is quite complex with multiple dependencies or risks.    | Rewriting a major component of the backend to accommodate a new hardware device and ensuring data consistency.          | High                                | High level of uncertainty and potential hurdles.|
| 13           | High effort with significant unknowns. Complex task with uncertainty.      | Migrating the entire backend infrastructure to a new platform while maintaining compatibility with existing hardware. | High                                | Substantial uncertainty and high risk.        |
| 21           | Very high effort with substantial unknowns. Extremely complex and risky.   | Designing and implementing a comprehensive security overhaul for the entire system, including hardware encryption.     | Very High                           | Extremely uncertain and high-risk endeavor.   |


## Acceptance Criteria
### Update Configuration Remotely via Event-Driven

| No. | Acceptance Criteria                                                                                          |
|-----|------------------------------------------------------------------------------------------------------------|
| 1.  | The embedded system should receive configuration update requests from the backend.                      |
| 2.  | Configuration updates should be initiated by an event from the backend, like an API call or a message.   |
| 3.  | Secure and efficient communication protocols (e.g., HTTPS or MQTT) should be used for updates.          |
| 4.  | Only authorized users/systems should trigger updates using authentication tokens or keys.             |
| 5.  | Configuration data must adhere to a specified format or schema understood by the embedded system.      |
| 6.  | Received configuration updates should be processed and applied by the embedded system.                 |
| 7.  | Proper error handling should manage cases of invalid or incomplete configuration data.                |
| 8.  | Configuration data should be validated for correctness and coherence before application.                |
| 9.  | Configuration updates should be compatible with the current embedded software version.                 |
| 10. | A mechanism should allow reverting to the previous configuration in case of issues or failures.       |
| 11. | Events related to configuration updates, successful or erroneous, should be logged.                    |
| 12. | Peripheral interactions should be managed appropriately if updated configurations affect peripherals.   |
| 13. | Test cases must cover successful updates, invalid data, network disruptions, and rollback scenarios.   |
| 14. | Detailed documentation should outline the event-driven update process, authentication, and errors.    |
| 15. | Evaluate the impact of updates on system performance to ensure no disruptions during normal operation. |


## Definition of Done

| Criteria     | Definition of Done for Embedded Systems                              |
|--------------|--------------------------------------------------------------------|
| Code         | Code developed, reviewed, and committed.                            |
| Compilation  | Code compiles successfully for the target hardware.                |
| Testing      | Unit and integration tests validate code and hardware.             |
| Safety       | Code adheres to safety standards.                                   |
| Documentation| Detailed technical and user documentation provided.                |
| Traceability | Requirements traceable and aligned.                                |
| Review       | Code and design reviewed and approved.                              |
| Deployment   | Software deployed on target hardware.                               |
| Validation   | System functionality validated against requirements.               |
| Acceptance   | Acceptance tests meet customer expectations.                        |
| Compliance   | Regulatory, security, and performance compliance achieved.         |
| Release      | Software ready for production deployment with documentation.      |
