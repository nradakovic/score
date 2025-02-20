..
   # *******************************************************************************
   # Copyright (c) 2025 Contributors to the Eclipse Foundation
   #
   # See the NOTICE file(s) distributed with this work for additional
   # information regarding copyright ownership.
   #
   # This program and the accompanying materials are made available under the
   # terms of the Apache License Version 2.0 which is available at
   # https://www.apache.org/licenses/LICENSE-2.0
   #
   # SPDX-License-Identifier: Apache-2.0
   # *******************************************************************************

Workproducts
============


.. _wp_traceability_model:

.. figure:: _assets/wp_traceability_model.drawio.svg
  :width: 100%
  :align: center
  :alt: Project work product traceability model

  Project development work product traceability model


Platform management
--------------------

General
^^^^^^^

.. workproduct:: Policies
   :id: wp_policies
   :status: draft
   :tags: requirements_management

   Organization-specific rules and processes for functional safety and cybersecurity.

.. workproduct:: Training path
   :id: wp_training_path
   :status: draft
   :tags: safety

   Evidence of competence management.

.. workproduct:: Quality management system
   :id: wp_qms
   :status: draft
   :tags: safety

   Evidence of quality management.

.. workproduct:: Quality report
   :id: wp_qms_report
   :status: draft
   :tags: safety

   | Evidence of quality conformance:
   | * Identifies what tasks/activities/process produce the information
   | * Identifies when the data was collected
   | * Identifies source of any associated data
   | * Identifies the associated quality criteria
   | * Identifies any associated measurements using the information

.. workproduct:: Issue tracking system
   :id: wp_issue_track_system
   :status: draft
   :tags: requirements_management, safety_management

   | - Identified safety anomaly reports
   | - Change requests (= Contribution Request)
   | - Impact analysis
   | - change request plan
   | - Change report
   |
   | Safety anomaly: Conditions that deviate from expectations and that can lead to harm.
   | The documentation of a change shall contain the list of changed work products, the details of the change and the planned date of deployment of the change.

.. workproduct:: Feature Request
   :id: wp_feat_request
   :status: draft
   :tags: contribution_management, safety_management

   | - Feature request
   | - Change request

.. workproduct:: Platform Management Plan
   :id: wp_platform_mgmt
   :status: draft
   :tags: safety_management

   The Platform Management Plan shall include the Project Management Plan, Configuration Management Plan, Change Management Plan, Documentation Management Plan and Problem Resolution Plan.
   Plan to ensure that all work products can be uniquely identified and reproduced in a controlled manner at any time.
   Plan to ensure that relations and differences between versions can be traced.
   Plan to manage, analyse and control changes of the work products during the project life cycle.
   Documents should be precise, concise, clearly structured, understandable for intended users, verifiable, maintainable, and organized according to in-house procedures to facilitate information retrieval.
   Documentation guideline requirements must be defined for each WP. Each work product or document must include a title, author and approver, unique revision identification, change history, and status.

.. workproduct:: Software Development Plan
   :id: wp_sw_dev_plan
   :status: draft
   :tags: process

   | Process description of SW development including
   | - selection of design and programming language
   | - design guideline
   | - coding guideline (e.g. MISRA, can also include style guide or naming convention)
   | - SW configuration guideline
   | - Method selection (e.g. for Architecture Verification)
   | - development tools
   |
   | Compare also `Gitub documentation <https://docs.github.com/en>`_
   | Compare also `Eclipse Project Handbook <https://www.eclipse.org/projects/handbook/>`_


Process
^^^^^^^

.. workproduct:: Process Definition
   :id: wp_process_definition
   :status: draft
   :tags: process

   Process definitions.

.. workproduct:: Process Improvement Report
   :id: wp_process_impr_report
   :status: draft
   :tags: process

   Process improvement report.

.. workproduct:: Process Management Strategy
   :id: wp_process_plan
   :status: draft
   :tags: process

   Plan to manage and guide execution of the process management activities.


Product development
-------------------

Platform development
^^^^^^^^^^^^^^^^^^^^

.. workproduct:: Stakeholder Requirements
   :id: wp_stakeholder_req
   :status: draft
   :tags: requirements_management

   Technical requirements from a stakeholder viewpoint and Assumptions of use based on the integration as SW platform SEooC in an assumed context.

.. workproduct:: Tool Requirements
   :id: wp_tool_req
   :status: draft
   :tags: requirements_management

   SW Requirements for tools to ensure automatic enforcement of rules and as input for software tool qualification.

.. workproduct:: Feature Requirements
   :id: wp_feature_req
   :status: draft
   :tags: requirements_management

   SW Requirements describing in a more detailed way the functionality which will fulfill a set of stakeholder requirements. A "feature" consists of a set of requirements. These feature requirements shall also be the basis for integration testing on platform level.

.. workproduct:: Feature Assumptions of Use
   :id: wp_feature_aou
   :status: draft
   :tags: safety

   SW Safety Requirements for the user of the feature, exportable requirements for the user to integrate in their req mgt system.

.. workproduct:: Feature Architecture
   :id: wp_feature_architecture
   :status: draft
   :tags: safety

   Feature Architecture linked to Feature Requirements, i.e. interaction of components
   - Static view (UML) - Feature interfaces (to outside of Feature) and Interfaces between own Components
   - Dynamic view (UML) - Sequences of component interactions and state diagrams

   Technical concept on platform level.

.. workproduct:: Feature Safety Analyses
   :id: wp_feature_safety_analyses
   :status: draft
   :tags: safety

   Bottom-Up Safety Analysis with e.g. FMEA method, verifies the feature architecture (as part of SW Safety Concept)
   - Detection and prevention mitigations linked to Software Feature Requirements or Assumptions of Use

.. workproduct:: Feature DFA
   :id: wp_feature_dfa
   :status: draft
   :tags: safety

   Dependent Failure Analysis on platform/feature level
   - Detection and prevention mitigations linked to Software Feature Requirements or Assumptions of Use
   Perform analysis on interactions between safety related and non-safety related modules or modules with different ASIL of one feature. Including potential influences from the rest of the SW platform.

.. workproduct:: Platform Build Configuration
   :id: wp_platform_sw_build_config
   :status: draft
   :tags: safety

   Build configuration capable to create the SEooC Library for the reference HW, platform level.
   Note: Embedded software in the sense of the Iso (i.e. deployed on the production HW) is not part of our delivery.

.. workproduct:: Feature Integration test
   :id: wp_feature_integration_test
   :status: draft
   :tags: safety

   Integration Testing verifies feature requirements and architecture:
   - all interfaces from Static view and
   - all flows from Dynamic View and
   - performance: i.e. RAM and processor usage
   on reference HW

.. workproduct:: Platform test
   :id: wp_platform_test
   :status: draft
   :tags: safety

   Platform Testing verfies Stakeholder Requirements performed on reference HW

.. workproduct:: Platform Verification Report
   :id: wp_platform_sw_verification_report
   :status: draft
   :tags: safety

   Verification Report contains:
   - List of requirements (and architecture/detailed design tags) tested by which test (can be several levels), passed/failed and completeness verdict, including normal operation and failure reactions
   - The list of requirements may also contain other verification methods like "Analysis"
   - Formal evidence about the preformed DFA.
   - Formal evidence about the performed Safety Analyses

.. workproduct:: Platform Release Notes
   :id: wp_platform_sw_release_note
   :status: draft
   :tags: safety_management

   Release notes describe the qualified SW version including known bugs from own testing and field reporting, with clear statement, that these bugs do not lead to violation of any safety requirements or with corresponding workaround measures. Platform level.


Component development
^^^^^^^^^^^^^^^^^^^^^

.. workproduct:: Component Requirements
   :id: wp_sw_component_req
   :status: draft
   :tags: requirements_management

   | SW Requirements for own and OSS qualified components/libraries. QM and ASIL requirements are distinguished by attributes/tags.

.. workproduct:: Component Assumptions of Use
   :id: wp_sw_component_aou
   :status: draft
   :tags: safety

   SW Safety Requirements for the user of the component, exportable requirements for the user to integrate in their req mgt system.

.. workproduct:: Hardware-software interface (HSI) specification
   :id: wp_hsi
   :status: draft
   :tags: safety

   | The HSI specification shall specify the hardware and software interaction and be consistent with the technical safety concept.
   | The HSI specification shall include the component's hardware parts that are controlled by software and hardware resources that support the execution of the software.

.. workproduct:: Requirements Inspection
   :id: wp_sw_req_inspect
   :status: draft
   :tags: safety

   | Depends on requirements management tooling, expect text based requirements maintained in git.
   | - github review with integrated inspection checklist, only valid requirements get merged
   |
   | Compare also `Gitub documentationt <https://docs.github.com/en>`_

.. workproduct:: Component Architecture
   :id: wp_sw_component_architecture
   :status: draft
   :tags: safety

   Component Architecture linked to Component Requirements
   - Static view (UML) - Component interfaces (to outside of Component) and Interfaces between own Sub-Components
   - Dynamic view (UML) - Sequences of Sub-Components interactions and Components States
   Note: In case no sub-components exist, this can be covered by Detailed Design (in "Implementation" workproduct)

.. workproduct:: Component Safety Analyses
   :id: wp_sw_component_safety_analyses
   :status: draft
   :tags: safety

   Bottom-Up Safety Analysis with e.g. FMEA method, verifies the component architecture (as part of SW Safety Concept)
   - Detection and prevention mitigations linked to Software Component Requirements or Assumptions of Use

.. workproduct:: Component DFA
   :id: wp_sw_component_dfa
   :status: draft
   :tags: safety

   Dependent Failure Analysis on component/module level
   - Detection and prevention mitigations linked to Software Component Requirements or Assumptions of Use
   Perform analysis of safety related and non-safety related sub-elements or sub-elements with different ASIL.
   Perform analysis on interactions between safety related and non-safety related sub-components or sub-components with different ASIL of one component. Including potential influences from the other components in the component's module.

.. workproduct:: Architecture Verification
   :id: wp_sw_arch_verification
   :status: draft
   :tags: safety

   Depends on architecture, FMEA and DFA tooling.
   May include several methods like inspection, modelling ... Which are selected in SW Development Plan.

.. workproduct:: Implementation
   :id: wp_sw_implementation
   :status: draft
   :tags: safety

   Implementation includes source code and detailed design (e.g. in form of comments or linked graphical representations) and SW configuration (e.g. #ifdef)
   The "how to" is described in the SW Development Plan guidelines

.. workproduct:: Unit test
   :id: wp_sw_unit_test
   :status: draft
   :tags: safety

   Unit testing verifies component requirements and detailed design (traced to). Tooling defined in SW Development Plan and integrated in CI/Build.

.. workproduct:: Code Inspection
   :id: wp_sw_code_inspect
   :status: draft
   :tags: safety

   github review with integrated inspection checklist (includes manual checking of coding guidelines)

.. workproduct:: Module Verification Report
   :id: wp_module_sw_verification_report
   :status: draft
   :tags: safety

   Verification Report contains:
   - List of requirements (and architecture/detailed design tags) tested by which test (can be several levels), passed/failed and completeness verdict, including normal operation and failure reactions
   - The list of requirements may also contain other verification methods like "Analysis"
   - Structural Coverage (C0 and C1, from unit testing on host) per unit
   - Static Code Analysis (including compiler warnings, automated checking of coding guidelines and additional checks)
   - Formal evidence about the preformed DFA.
   - Formal evidence about the performed Safety Analyses
   - Software component qualification verification report

.. workproduct:: Component Integration test
   :id: wp_sw_component_integration_test
   :status: draft
   :tags: safety

   Integration Testing verifies component architecture:
   - all interfaces from Static view and
   - all flows from Dynamic View and
   performance: i.e. RAM and processor usage on reference HW

.. workproduct:: Module Build Configuration
   :id: wp_module_sw_build_config
   :status: draft
   :tags: safety

   Build configuration capable to create the SEooC Library for the reference HW, module level.
   Note: Embedded software in the sense of the Iso (i.e. deployed on the production HW) is not part of our delivery.

.. workproduct:: Module Release Notes
   :id: wp_module_sw_release_note
   :status: draft
   :tags: safety_management

   Release notes describe the qualified SW version including known bugs from own testing and field reporting, with clear statement, that these bugs do not lead to violation of any safety requirements or with corresponding workaround measures. Module level.


.. workproduct:: Component test
   :id: wp_sw_component_test
   :status: draft
   :tags: safety

   Component Testing verifies Component Requirements


Supporting activities
---------------------

.. workproduct:: Verification Plan
   :id: wp_verification_plan
   :status: draft
   :tags: process, safety

   Verification planning for each phase of the safety lifecycle must detail the work products, objectives, methods, criteria, environments, equipment, resources, actions for anomalies, and regression strategies, considering method adequacy, complexity, prior experiences, and technology maturity or risks.

.. workproduct:: Verification Specification
   :id: wp_verification_spec
   :status: draft
   :tags: process, safety

   The verification specification must outline the verification methods, including review or analysis checklists, simulation scenarios.
   Test cases, test data, and test objects are part of the respective test WPs.

.. workproduct:: Software tool criteria evaluation report
   :id: wp_tool_eval
   :status: draft
   :tags: process, safety

   According to the tool evaluation process, each tool's confidence level (TCL) must be determined. Based on TCL the appropriate qualification methods shall be applied.


Note: All the work products are set to status "draft", as the linkage to standard requirements is missing currently on purpose, namely to those of ISO 26262.
