# Administering the Capstone Course

This document covers how to create and configure new instances of the CS Capstone course.

## Directory Structure

- `assignments/` — Markdown files with YAML metadata describing each assignment posted in Canvas
- `content/` — Detailed course content (long-form descriptions, resource lists, guides). Originals are in Markdown, rendered to HTML or PDF where needed.
- `files/` — Static files (PDFs, presentations, videos) distributed through Canvas
- `issues/` — GitHub Issues for a private course Kanban board covering developer checkpoints, discussions, and instructor deliverables
- `quizzes/` — Markdown files with YAML metadata describing each quiz posted in Canvas
- `modules.yaml` — Defines the Canvas module structure and item ordering
- `course-info.yaml` — Per-instance course configuration (section, semester, CRN, etc.)

## Creating a New Course Instance

Course provisioning uses MosTidy's Canvas commands. See the [MosTidy Canvas Course Templates documentation](../../__program/MosTidy/docs/canvas-course-templates.md) for current usage.

```bash
# Extract templates from an existing course
mostidy canvas extract <source_course_id> -o ./

# Preview what will be created
mostidy canvas insert . --course <new_course_id> --config course-info.yaml --dry-run

# Create content in new course
mostidy canvas insert . --course <new_course_id> --config course-info.yaml
```

To create a new semester instance, create a branch of this repo named with the course number, section number, semester code, and CRN delimited by hyphens (e.g., `csci-4961-01-262-12345`). Update `course-info.yaml` with any fields labeled `required`.
