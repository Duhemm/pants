# Copyright 2019 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

python_library(
  dependencies=[
    '3rdparty/python:dataclasses',
    'src/python/pants/backend/python/lint',
    'src/python/pants/backend/python/subsystems',
    'src/python/pants/backend/python/rules',
    'src/python/pants/engine:fs',
    'src/python/pants/engine:isolated_process',
    'src/python/pants/engine:rules',
    'src/python/pants/engine:selectors',
    'src/python/pants/option',
    'src/python/pants/python',
    'src/python/pants/rules/core',
  ],
  tags = {"partially_type_checked"},
)

python_tests(
  name='integration',
  sources=['*_integration_test.py'],
  dependencies=[
    ':black',
    'src/python/pants/backend/python/lint',
    'src/python/pants/backend/python/subsystems',
    'src/python/pants/engine:fs',
    'src/python/pants/engine:rules',
    'src/python/pants/engine:selectors',
    'src/python/pants/engine/legacy:structs',
    'src/python/pants/rules/core',
    'src/python/pants/source',
    'src/python/pants/testutil:test_base',
    'src/python/pants/testutil/option',
  ],
  tags = {'integration', 'partially_type_checked'},
)
