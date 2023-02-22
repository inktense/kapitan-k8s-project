# My Readme

Target: my_target

# INVENTORY

```
- common
- my_component

```


```
_reclass_:
  environment: base
  name:
    full: my_target
    short: my_target
kapitan:
  compile:
  - input_paths:
    - components/my_component/my_component.jsonnet
    input_type: jsonnet
    output_path: jsonnet_output
    output_type: yaml
  - input_paths:
    - templates/scripts
    input_type: jinja2
    output_path: scripts
  - input_paths:
    - templates/docs
    input_type: jinja2
    output_path: .
    output_type: yaml
  - input_paths:
    - components/other_component/
    input_type: kadet
    output_path: kadet_output
    output_type: yaml
  vars:
    target: my_target
target_name: my_target
your_component:
  some_parameter: true

```