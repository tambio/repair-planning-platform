# Verification and Evaluation Plan

## 1. Introduction
This document describes how we will test the platform and measure its success. The goal is to show that the system meets the requirements and helps users.

## 2. Testing Approach

We use three types of testing:

1. **Unit testing** — test each module separately.
2. **Integration testing** — test how modules work together.
3. **User testing** — test with real users (builder and client).

## 3. Test Plan by Module

### 3.1 Auth Module
- Test: register, login, logout, role check.
- Tools: pytest, FastAPI TestClient.
- Success: user can register and log in, role is correct.

### 3.2 Cost Calculation Module
- Test: calculate cost for different work types and areas.
- Tools: pytest.
- Success: cost matches manual calculation (error < 1%).

### 3.3 AI Planning Module
- Test: build schedule for a project with dependencies and pauses.
- Tools: pytest, manual check.
- Success: schedule has no conflicts, pauses are correct.

### 3.4 Receipt Module
- Test: upload receipt, enter expense, assign category.
- Tools: pytest, manual check.
- Success: expense is saved and shown in analytics.

### 3.5 Analytics Module
- Test: plan vs fact calculation, forecast.
- Tools: pytest.
- Success: numbers match manual calculation.

## 4. Evaluation Metrics

| Metric | How to Measure | Target |
|--------|----------------|--------|
| Cost calculation accuracy | Compare with manual Excel calculation | Error < 1% |
| Schedule building time | Time to build schedule in platform vs manual | In platform is 5x faster |
| Schedule conflicts | Number of conflicts in schedule | 0 conflicts |
| Expense entry time | Time to add one expense | < 30 seconds |
| User satisfaction | Survey after testing (1–5) | Average > 4 |
| System response time | Measure API response | < 2 seconds |

## 5. Baseline for Comparison

To show the value of the platform, we compare it with the current manual method:

| Task | Manual (Excel) | Our Platform |
|------|----------------|--------------|
| Calculate cost | 1–2 hours | 5–10 minutes |
| Build schedule | 1–2 hours | 1–2 minutes |
| Track expenses | Hard, no system | Easy, with categories |
| Plan vs fact | Manual, often forgotten | Automatic |

## 6. User Testing Plan

We will test the platform with:
- 2–3 private builders,
- 2–3 clients who did renovation recently.

Test scenario:
1. Builder creates a project.
2. Builder calculates cost and builds schedule.
3. Client views shopping list.
4. Client uploads receipts and enters expenses.
5. Both view analytics.

After testing, we ask users to fill a short survey.

## 7. Success Criteria

The project is successful if:
- All "Must" requirements are implemented and tested.
- Cost calculation error is less than 1%.
- Schedule has no conflicts.
- Users rate the platform 4 or higher.
- System response time is less than 2 seconds.

## 8. Conclusion

This plan shows how we will verify the platform. It covers unit tests, integration tests, and user testing. It also defines clear metrics and a baseline for comparison.