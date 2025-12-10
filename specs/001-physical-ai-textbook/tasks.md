# Tasks: Physical AI & Humanoid Robotics Textbook

**Input**: Design documents from `specs/001-physical-ai-textbook/`
**Prerequisites**: plan.md, spec.md

## Phase 1: Setup

**Purpose**: Project initialization and basic structure.

- [X] T001 Initialize a new Docusaurus project with the classic-typescript template.
- [X] T002 Update `docusaurus.config.ts` with the title 'Panaversity Physical AI Textbook', a tagline, and a placeholder logo path.
- [X] T003 Update `src/css/custom.css` with basic branding colors for Panaversity.
- [X] T004 Modify the homepage at `src/pages/index.tsx` to reflect the textbook's title and purpose.

---

## Phase 2: Foundational (Content Structure)

**Purpose**: Create the directory and placeholder files for all modules.

- [X] T005 [P] Create directory `docs/01-introduction-to-physical-ai`.
- [X] T006 [P] Create `docs/01-introduction-to-physical-ai/_category_.json` with a label "1. Introduction to Physical AI".
- [X] T007 [P] Create placeholder file `docs/01-introduction-to-physical-ai/01-intro.md`.
- [X] T008 [P] Create directory `docs/02-ros-2-fundamentals`.
- [X] T009 [P] Create `docs/02-ros-2-fundamentals/_category_.json` with a label "2. ROS 2 Fundamentals".
- [X] T010 [P] Create placeholder file `docs/02-ros-2-fundamentals/01-intro.md`.
- [X] T011 [P] Create directory `docs/03-robot-simulation`.
- [X] T012 [P] Create `docs/03-robot-simulation/_category_.json` with a label "3. Robot Simulation (Digital Twin)".
- [X] T013 [P] Create placeholder file `docs/03-robot-simulation/01-intro.md`.
- [X] T014 [P] Create directory `docs/04-the-ai-robot-brain`.
- [X] T015 [P] Create `docs/04-the-ai-robot-brain/_category_.json` with a label "4. The AI-Robot Brain (NVIDIA Isaac)".
- [X] T016 [P] Create placeholder file `docs/04-the-ai-robot-brain/01-intro.md`.
- [X] T017 [P] Create directory `docs/05-humanoid-robot-development`.
- [X] T018 [P] Create `docs/05-humanoid-robot-development/_category_.json` with a label "5. Humanoid Robot Development".
- [X] T019 [P] Create placeholder file `docs/05-humanoid-robot-development/01-intro.md`.
- [X] T020 [P] Create directory `docs/06-conversational-robotics`.
- [X] T021 [P] Create `docs/06-conversational-robotics/_category_.json` with a label "6. Conversational Robotics (VLA)".
- [X] T022 [P] Create placeholder file `docs/06-conversational-robotics/01-intro.md`.
- [X] T023 Configure `sidebars.ts` to auto-generate the sidebar from the `docs` directory structure.

---

## Phase 3: Content - Foundational Modules

**Purpose**: Write the initial content for the first three modules.

- [X] T024 [P] [US3] Write content for "Embodied Intelligence" in `docs/01-introduction-to-physical-ai/01-intro.md`.
- [X] T025 [P] [US3] Write 2500+ words on ROS 2 in `docs/02-ros-2-fundamentals/01-intro.md`. Must cover: Middleware architecture, Nodes vs Topics vs Services, coding a 'talker/listener' in Python with `rclpy`, and detailed explanation of URDF for humanoids.
- [X] T026 [P] [US3] Write 2500+ words on Simulation in `docs/03-robot-simulation/01-intro.md`. Must cover: Physics/Gravity engines in Gazebo, importing URDF/SDF, Unity visualization, and simulating specific sensors (LiDAR, Depth Cameras, IMUs).

---

## Phase 4: Content - Advanced Modules

**Purpose**: Write the initial content for the last three modules.

- [X] T027 [P] [US3] Write 2500+ words on NVIDIA Isaac in `docs/04-the-ai-robot-brain/01-intro.md`. Must cover: Isaac Sim setup, Synthetic Data Generation, VSLAM hardware acceleration, and Nav2 path planning.
- [X] T028 [P] [US3] Write content for "Humanoid Kinematics" in `docs/05-humanoid-robot-development/01-intro.md`.
- [X] T029 [P] [US3] Write 2500+ words on Vision-Language-Action in `docs/06-conversational-robotics/01-intro.md`. Must cover: OpenAI Whisper integration, Cognitive Planning (LLM to ROS 2 translation), and the 'Autonomous Humanoid' capstone logic.

---

## Phase 5: Polish & Deployment

**Purpose**: Finalize the project and set up deployment.

- [X] T030 Configure `docusaurus.config.ts` for GitHub Pages deployment.
- [X] T031 Create a GitHub Actions workflow file at `.github/workflows/deploy.yml` to build and deploy the site.

---
## Dependencies & Execution Order

- **Phase 1 (Setup)** must be completed before all other phases.
- **Phase 2 (Foundational)** depends on Phase 1.
- **Phase 3 & 4 (Content)** can be done in parallel after Phase 2 is complete.
- **Phase 5 (Deployment)** is the final step.

## Implementation Strategy

### MVP First (User Story 1 & 2)

1.  Complete Phase 1: Setup
2.  Complete Phase 2: Foundational
3.  **STOP and VALIDATE**: The site should be running with correct branding and the sidebar should be functional with placeholders.

### Incremental Delivery

1.  After MVP, content from Phase 3 and 4 can be added incrementally.
2.  Once all content is ready, Phase 5 can be completed to deploy the site.
