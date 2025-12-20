---
layout: project
title: Ethics & the Boeing 737 Max & Ethics
image: /assets/images/plane.jpg
---
## Ethical Decision-Making and Design Failure in the Boeing 737 MAX

In October 2018 and March 2019, two Boeing 737 MAX aircraft crashed shortly after takeoff, killing all passengers and crew aboard. The immediate cause in both accidents was the activation of the Maneuvering Characteristics Augmentation System (MCAS), flight control software designed to prevent stall introduced by the 737 MAX’s new, larger, repositioned engines. While the triggering failure involved faulty Angle of Attack (AOA) sensor data, the accidents were ultimately the result of a sequence of ethical and organizational decisions made during design, certification, and testing.

#### Issue 1: The Southwest Deal and the Pressure Cooker

Boeing developed the 737 MAX under intense competitive pressure to counter Airbus’s A320neo. This pressure was amplified by Boeing’s relationship with Southwest Airlines. Early in the design process, Boeing committed to delivering an aircraft at approximately one million dollars per plane, which significantly constrained design choices and created an environment in which avoiding more expensive pilot training became a primary design objective.

This deal created what Boeing engineer Rick Ludtke described as a *“pressure cooker”* that fundamentally altered business and engineering values throughout the entire design process. This represents a clear conflict between engineering ethics and business priorities. The agreement with Southwest was made too early, before Boeing fully understood how design changes would cascade into safety-critical issues.


#### Issue 2: Hiding MCAS from Pilots and Regulators

Rather than creating a new aircraft design, Boeing modified the existing 737 airframe, introducing new aerodynamic characteristics that required later design compensation. The repositioned, heavier engines and changes to lift characteristics altered the aircraft’s pitch behavior at high angles of attack.

MCAS was initially presented to FAA regulators as a small modification to an existing trim system, but it was later expanded to activate during takeoff with the ability to repeatedly command the nose downward. Boeing’s chief technical pilot, Mark Forkner, emailed the FAA requesting that MCAS be removed from the pilot training manual. Forkner later admitted in internal messages that he “basically lied to the FAA, unknowingly,” yet he never corrected this misinformation.

As a result, MCAS was not treated as a high-risk system and received limited scrutiny during certification, largely due to how Boeing characterized the system to regulators.

#### Issue 3: The Single AOA Sensor Design Flaw

The MCAS software was introduced to address pitch-up characteristics, but Boeing classified unintended MCAS activation as a “Major” failure rather than “Hazardous” or “Catastrophic” in its internal certification documentation (U.S. Department of Transportation, 2020). This classification did not require design redundancy and allowed MCAS to rely on input from a single AOA sensor: a poor design choice given that AOA sensors are known to be unreliable.

Subsequent investigations concluded that this single-sensor dependency was a central contributing factor in both crashes (Herkert et al., 2020; U.S. Department of Transportation, 2020).

Using a single known-fault-prone sensor violates established engineering best practices. Aircraft systems are typically built with redundancy: two pilots, multiple control paths, and multiple sensors. This fundamental design flaw cascaded into catastrophic consequences.

#### Issue 4: Expanding MCAS Without FAA Notification

Boeing’s decision to expand MCAS to operate during takeoff without informing the FAA demonstrated a knowing abuse of the certification and verification process and was a direct cause of the crashes. Had MCAS not been expanded to function during takeoff, the two crashes would not have occurred.

Boeing assessed unintended MCAS activation as a “Major” failure, which did not require redundancy. Boeing also treated its failure probability analysis as an internal document and did not submit it as a certification deliverable.

The FAA delegated 28 of 87 certification activities, approximately one-third, back to Boeing under the Organization Designation Authorization (ODA) program, including MCAS-related certification. While this delegation had precedent, the MAX program demonstrated how internal review can compromise safety when combined with intense commercial pressure.

#### Issue 5: The Culture of Silence

Following the first crash, engineers raised concerns that were not escalated within the organization. Joe Jacobsen, an FAA engineer who analyzed the first crash, identified MCAS as the primary design flaw and reported it to three managers. However, all were skeptical, and the issue was never escalated.

Pilot training was classified as Level B, consisting primarily of slide presentations and computer-based instruction. Pilots were unprepared for MCAS failures and were unable to effectively override MCAS activation.

Boeing also failed to directly notify the FAA about the AOA alert issue, determining internally that it posed “no organizational impact.” Operators were given until June 18, 2019, to install a software fix finalized on February 13, 2019, allowing the Ethiopian Airlines crash to occur in the interim.

#### Conclusion

Ultimately, the Boeing 737 MAX crashes were not the result of a single technical error, but the culmination of ethical failures stemming from design tradeoffs, regulatory shortcomings, organizational silence, and overwhelming commercial pressure.

---

#### References

- Herkert, J. R., Borenstein, J., & Miller, K. (2020). *The Boeing 737 MAX: Lessons for engineering ethics*. Science and Engineering Ethics, 26, 2957–2974.  
- U.S. Department of Transportation, Office of Inspector General. (2020). *FAA oversight of Boeing 737 MAX certification*.
