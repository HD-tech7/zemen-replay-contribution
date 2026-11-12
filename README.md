# ZEMEN — REPLAY COURT CONTRIBUTION

**Individual Contribution Portfolio — INSA Submission**

| Information | Details |
|---|---|
| Contributor | Hundaol Dechassa |
| Student ID | CTC-582-26 |
| Project | Zemen |
| Contribution | Replay Court |
| Demonstration | [Watch on YouTube](https://youtu.be/G-G8kOnDHkU) |

---

## 1. Project Overview

Zemen is a security detection integrity and Ethiopian temporal-context platform designed to work with OpenSearch and Wazuh.

The project contains different modules that improve security monitoring, detection verification, and security analytics.

My individual contribution focuses on the **Replay Court subsystem**.

## 2. What Is Replay?

In Zemen, Replay is a controlled process of submitting prepared security-event records into a dedicated test environment to verify whether configured security detectors respond correctly.

Replay Court makes it possible to test detector behavior repeatedly and record the results.

It provides a practical way to verify detection performance instead of simply assuming that a configured detector is working.

## 3. My Contribution to Zemen

| No. | Contribution Area | Description |
|---|---|---|
| 1 | Replay Case Management | Preparation and organization of replay test cases |
| 2 | Case Validation | Checking replay case requirements |
| 3 | Event Replay | Submitting prepared test events |
| 4 | Detector Verification | Checking whether expected detectors produce findings |
| 5 | Result Management | Recording replay execution results |
| 6 | Performance Measurement | Measuring detector response time |
| 7 | Replay Safety | Supporting separate replay test data and cleanup |
| 8 | Testing | Validation of replay cases and safety rules |

## 4. How Replay Works

1. A replay test case is prepared.
2. The system validates the test case.
3. The target test index is checked.
4. Prepared events are submitted.
5. Zemen checks for the expected detector finding.
6. The result and response time are recorded.
7. Replay test data can be cleaned up according to the configured behavior.

## 5. Replay Results

| Status | Meaning |
|---|---|
| PASS | Expected detector finding was observed |
| FAIL | No matching finding was observed within the configured period |
| PARTIAL | Some detector checks passed and others did not |
| ERROR | The replay case could not be executed successfully |

## 6. Technical Implementation

Important source locations in the Zemen project:

- `internal/replay/replay.go`
- `internal/replay/replay_test.go`
- `internal/pipeline/pipeline.go`
- `internal/web/server.go`
- `cmd/zemen/commands.go`
- `internal/indices/mappings.go`

These files show the Replay implementation and its connections with the wider Zemen application.

## 7. Video Demonstration

Click the image below to watch my Zemen demonstration.

[![Watch Zemen Replay Demonstration](https://img.youtube.com/vi/G-G8kOnDHkU/hqdefault.jpg)](https://youtu.be/G-G8kOnDHkU)

**Video:** https://youtu.be/G-G8kOnDHkU

## 8. Contribution Value

Replay Court improves the reliability of security monitoring by providing a repeatable way to verify detector behavior.

It helps the project team:

- Verify whether configured detectors respond to prepared test events.
- Identify possible detection problems.
- Measure detector response time.
- Maintain records of validation results.
- Improve confidence in security monitoring.

## 9. Conclusion

My contribution to Zemen focuses on the Replay Court feature.

This contribution supports the project's objective of improving security detection reliability through controlled testing, verification, and measurable results.

I acknowledge that Zemen is a team project and that my individual contribution is focused on Replay rather than the entire application.

**Contributor:** Hundaol Dechassa  
**ID:** CTC-582-26
