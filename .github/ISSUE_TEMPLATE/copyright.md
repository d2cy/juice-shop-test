name: "🚨 Copyright Violation"
description: "Report a copyright violation detected by the scanning tool."
title: "🚨 Copyright Violation - <Brief Description>"
labels: ["copyright", "violation", "investigation"]
assignees: []

body:
  - type: input
    id: file_url
    attributes:
      label: "📄 File"
      description: "Provide the URL of the affected file."
      placeholder: "e.g., https://github.com/org/repo/blob/main/file.ext"
    validations:
      required: true

  - type: input
    id: copyright
    attributes:
      label: "© Copyright"
      description: "Describe the copyright violation (e.g., proprietary code used without permission)."
      placeholder: "e.g., Code copied from XYZ repository."
    validations:
      required: true

  - type: input
    id: line_number
    attributes:
      label: "📌 Line Number"
      description: "Specify the exact line number where the violation occurs."
      placeholder: "e.g., Line 42"
    validations:
      required: true
