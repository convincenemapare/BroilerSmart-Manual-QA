# BroilerSmart Manual QA Test Execution Summary

## 1. Objective

To evaluate the Create New Batch feature, focusing on input validation, unusual values, name handling, and saved records.

## 2. Test Environment

- Application: BroilerSmart
- Version: 1.0.0
- Device: Samsung A06 5G
- Operating system: Android 16
- Test dates: 7 October 2026 and 16 October 2026

## 3. Key Findings

- Empty batch names were rejected.
- Zero and negative bird quantities were rejected.
- Extremely large bird quantities were accepted and displayed in scientific notation.
- Repeated testing showed similar acceptance of unusually large quantities.
- Spaces-only supplier names were accepted in an earlier test.
- Special characters and emojis were tested in names; the specific observations need to be documented separately.
- Saved data remained available after leaving and reopening the application.

## 4. Assessment

The large-quantity finding indicates that the application currently lacks a clearly defined and documented maximum batch-size rule. This is recorded as a potential validation issue and improvement recommendation pending requirements and impact assessment.

Other findings must be assessed against documented requirements before being classified as defects.

## 5. Limitations

The intended maximum batch size has not yet been defined. The exact input used in the first large-quantity test is not known. Additional evidence and checks may be required.

## 6. Recommended Next Steps

1. Define appropriate business rules for batch quantities.
2. Document the expected handling of blank supplier names and unusual characters.
3. Test relevant boundary values after the rules are defined.
4. Review the results and update the defect or improvement records.

## 7. Status

Initial manual testing completed. Documentation and further validation are in progress.
