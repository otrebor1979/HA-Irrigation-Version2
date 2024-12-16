I don't use google Assistant but @genestealer has suggested this if you do:

(See below for a simplified option)

```
#################################################
# Google Assistant integration.
# Every now and again have to visit this link and lick TEST: https://console.actions.google.com/project/hassio-214617/accountlinking/
google_assistant:
  project_id: !secret google_assistant_project_id
  secure_devices_pin: !secret google_assistant_secure_devices_pin
  service_account: !include private/google_assistant_report_state_hassio_214617.json
  report_state: true
  entity_config:
    input_boolean.irrigation_cycle1_adjust_for_rainfall:
      expose: false
    input_boolean.irrigation_cycle1_adjust_for_temperature:
      expose: false
    input_text.irrigation_cycle1_name:
      expose: false
    input_boolean.irrigation_cycle1_running:
      expose: false
    input_boolean.irrigation_cycle1_schedule_enabled:
      expose: false
    input_boolean.irrigation_cycle1_schedule_today_only:
      expose: false
    input_datetime.irrigation_cycle1_start_time:
      expose: false
    input_boolean.irrigation_cycle1_wait_for_entity:
      expose: false
    input_number.irrigation_cycle1_zone1_duration_box:
      expose: false
    input_number.irrigation_cycle1_zone2_duration_box:
      expose: false
    input_number.irrigation_cycle1_zone3_duration_box:
      expose: false
    input_number.irrigation_cycle1_zone4_duration_box:
      expose: false
    input_number.irrigation_cycle1_zone1_duration:
      expose: false
    input_number.irrigation_cycle1_zone2_duration:
      expose: false
    input_number.irrigation_cycle1_zone3_duration:
      expose: false
    input_number.irrigation_cycle1_zone4_duration:
      expose: false
    input_boolean.irrigation_cycle1_zone1_every_day:
      expose: false
    input_boolean.irrigation_cycle1_zone1_fri:
      expose: false
    input_boolean.irrigation_cycle1_zone1_mon:
      expose: false
    input_boolean.irrigation_cycle1_zone1_sat:
      expose: false
    input_boolean.irrigation_cycle1_zone1_sun:
      expose: false
    input_boolean.irrigation_cycle1_zone1_thu:
      expose: false
    input_boolean.irrigation_cycle1_zone1_tue:
      expose: false
    input_boolean.irrigation_cycle1_zone1_wed:
      expose: false
    input_boolean.irrigation_cycle1_zone2_every_day:
      expose: false
    input_boolean.irrigation_cycle1_zone2_fri:
      expose: false
    input_boolean.irrigation_cycle1_zone2_mon:
      expose: false
    input_boolean.irrigation_cycle1_zone2_sat:
      expose: false
    input_boolean.irrigation_cycle1_zone2_sun:
      expose: false
    input_boolean.irrigation_cycle1_zone2_thu:
      expose: false
    input_boolean.irrigation_cycle1_zone2_tue:
      expose: false
    input_boolean.irrigation_cycle1_zone2_wed:
      expose: false
    input_boolean.irrigation_cycle1_zone3_every_day:
      expose: false
    input_boolean.irrigation_cycle1_zone3_fri:
      expose: false
    input_boolean.irrigation_cycle1_zone3_mon:
      expose: false
    input_boolean.irrigation_cycle1_zone3_sat:
      expose: false
    input_boolean.irrigation_cycle1_zone3_sun:
      expose: false
    input_boolean.irrigation_cycle1_zone3_thu:
      expose: false
    input_boolean.irrigation_cycle1_zone3_tue:
      expose: false
    input_boolean.irrigation_cycle1_zone3_wed:
      expose: false
    input_boolean.irrigation_cycle1_zone4_every_day:
      expose: false
    input_boolean.irrigation_cycle1_zone4_fri:
      expose: false
    input_boolean.irrigation_cycle1_zone4_mon:
      expose: false
    input_boolean.irrigation_cycle1_zone4_sat:
      expose: false
    input_boolean.irrigation_cycle1_zone4_sun:
      expose: false
    input_boolean.irrigation_cycle1_zone4_thu:
      expose: false
    input_boolean.irrigation_cycle1_zone4_tue:
      expose: false
    input_boolean.irrigation_cycle1_zone4_wed:
      expose: false
    input_boolean.irrigation_cycle2_adjust_for_rainfall:
      expose: false
    input_boolean.irrigation_cycle2_adjust_for_temperature:
      expose: false
    input_text.irrigation_cycle2_name:
      expose: false
    input_boolean.irrigation_cycle2_running:
      expose: false
    input_boolean.irrigation_cycle2_schedule_enabled:
      expose: false
    input_boolean.irrigation_cycle2_schedule_today_only:
      expose: false
    input_datetime.irrigation_cycle2_start_time:
      expose: false
    input_boolean.irrigation_cycle2_wait_for_entity:
      expose: false
    input_number.irrigation_cycle2_zone1_duration_box:
      expose: false
    input_number.irrigation_cycle2_zone2_duration_box:
      expose: false
    input_number.irrigation_cycle2_zone3_duration_box:
      expose: false
    input_number.irrigation_cycle2_zone4_duration_box:
      expose: false
    input_number.irrigation_cycle2_zone1_duration:
      expose: false
    input_number.irrigation_cycle2_zone2_duration:
      expose: false
    input_number.irrigation_cycle2_zone3_duration:
      expose: false
    input_number.irrigation_cycle2_zone4_duration:
      expose: false
    input_boolean.irrigation_cycle2_zone1_every_day:
      expose: false
    input_boolean.irrigation_cycle2_zone1_fri:
      expose: false
    input_boolean.irrigation_cycle2_zone1_mon:
      expose: false
    input_boolean.irrigation_cycle2_zone1_sat:
      expose: false
    input_boolean.irrigation_cycle2_zone1_sun:
      expose: false
    input_boolean.irrigation_cycle2_zone1_thu:
      expose: false
    input_boolean.irrigation_cycle2_zone1_tue:
      expose: false
    input_boolean.irrigation_cycle2_zone1_wed:
      expose: false
    input_boolean.irrigation_cycle2_zone2_every_day:
      expose: false
    input_boolean.irrigation_cycle2_zone2_fri:
      expose: false
    input_boolean.irrigation_cycle2_zone2_mon:
      expose: false
    input_boolean.irrigation_cycle2_zone2_sat:
      expose: false
    input_boolean.irrigation_cycle2_zone2_sun:
      expose: false
    input_boolean.irrigation_cycle2_zone2_thu:
      expose: false
    input_boolean.irrigation_cycle2_zone2_tue:
      expose: false
    input_boolean.irrigation_cycle2_zone2_wed:
      expose: false
    input_boolean.irrigation_cycle2_zone3_every_day:
      expose: false
    input_boolean.irrigation_cycle2_zone3_fri:
      expose: false
    input_boolean.irrigation_cycle2_zone3_mon:
      expose: false
    input_boolean.irrigation_cycle2_zone3_sat:
      expose: false
    input_boolean.irrigation_cycle2_zone3_sun:
      expose: false
    input_boolean.irrigation_cycle2_zone3_thu:
      expose: false
    input_boolean.irrigation_cycle2_zone3_tue:
      expose: false
    input_boolean.irrigation_cycle2_zone3_wed:
      expose: false
    input_boolean.irrigation_cycle2_zone4_every_day:
      expose: false
    input_boolean.irrigation_cycle2_zone4_fri:
      expose: false
    input_boolean.irrigation_cycle2_zone4_mon:
      expose: false
    input_boolean.irrigation_cycle2_zone4_sat:
      expose: false
    input_boolean.irrigation_cycle2_zone4_sun:
      expose: false
    input_boolean.irrigation_cycle2_zone4_thu:
      expose: false
    input_boolean.irrigation_cycle2_zone4_tue:
      expose: false
    input_boolean.irrigation_cycle2_zone4_wed:
      expose: false
    input_text.irrigation_cycle3_name:
      expose: false
    input_boolean.irrigation_cycle3_running:
      expose: false
    input_number.irrigation_cycle3_zone1_duration_box:
      expose: false
    input_number.irrigation_cycle3_zone2_duration_box:
      expose: false
    input_number.irrigation_cycle3_zone3_duration_box:
      expose: false
    input_number.irrigation_cycle3_zone4_duration_box:
      expose: false
    input_number.irrigation_cycle3_zone1_duration:
      expose: false
    input_number.irrigation_cycle3_zone2_duration:
      expose: false
    input_number.irrigation_cycle3_zone3_duration:
      expose: false
    input_number.irrigation_cycle3_zone4_duration:
      expose: false
    automation.irrigation_about_cycle_wifi_interruption:
      expose: false
    input_select.irrigation_cycle:
      expose: false
    input_text.irrigation_cycle1_wait_for_entity_name:
      expose: false
    input_text.irrigation_cycle1_wait_for_entity_state:
      expose: false
    input_boolean.irrigation_cycle1_wait_for_entity_name_timeout_continue:
      expose: false
    input_number.irrigation_cycle1_wait_for_entity_name_timeout_duration:
      expose: false
    input_text.irrigation_cycle2_wait_for_entity_name:
      expose: false
    input_text.irrigation_cycle2_wait_for_entity_state:
      expose: false
    input_boolean.irrigation_cycle2_wait_for_entity_name_timeout_continue:
      expose: false
    input_number.irrigation_cycle2_wait_for_entity_name_timeout_duration:
      expose: false
    automation.irrigation_cycle1_start_time_sunrise_offset:
      expose: false
    automation.irrigation_cycle1_start_time_sunset_offset:
      expose: false
    input_select.irrigation_cycle1_start_time_type:
      expose: false
    automation.irrigation_cycle2_start_time_sunrise_offset:
      expose: false
    automation.irrigation_cycle2_start_time_sunset_offset:
      expose: false
    input_select.irrigation_cycle2_start_time_type:
      expose: false
    automation.irrigation_notify_about_cycle_wifi_interruption:
      expose: false
    automation.irrigation_notify_when_cycle_starts_or_stops_2:
      expose: false
    automation.irrigation_notify_when_cycle_starts_or_stops:
      expose: false
    input_text.irrigation_previous_run_cycle_name:
      expose: false
    automation.irrigation_triggered_cycle_start:
      expose: false
    automation.irrigation_ui_set_default_cycle_names:
      expose: false
    group.irrigation_group_cycle1_every_day:
      expose: false
    group.irrigation_group_cycle1_fri:
      expose: false
    group.irrigation_group_cycle1_mon:
      expose: false
    group.irrigation_group_cycle1_sat:
      expose: false
    group.irrigation_group_cycle1_sun:
      expose: false
    group.irrigation_group_cycle1_thu:
      expose: false
    group.irrigation_group_cycle1_tue:
      expose: false
    group.irrigation_group_cycle1_wed:
      expose: false
    group.irrigation_group_cycle1_zone_durations:
      expose: false
    group.irrigation_group_cycle2_every_day:
      expose: false
    group.irrigation_group_cycle2_fri:
      expose: false
    group.irrigation_group_cycle2_mon:
      expose: false
    group.irrigation_group_cycle2_sat:
      expose: false
    group.irrigation_group_cycle2_sun:
      expose: false
    group.irrigation_group_cycle2_thu:
      expose: false
    group.irrigation_group_cycle2_tue:
      expose: false
    group.irrigation_group_cycle2_wed:
      expose: false
    group.irrigation_group_cycle2_zone_durations:
      expose: false
    group.irrigation_group_cycle3_zone_durations:
      expose: false
    input_boolean.irrigation_ui_show_cycle1:
      expose: false
    input_boolean.irrigation_ui_show_cycle2:
      expose: false
    input_boolean.irrigation_ui_show_cycle3:
      expose: false
    input_number.irrigation_cycle1_start_time_sunrise_offset:
      expose: false
    input_number.irrigation_cycle2_start_time_sunrise_offset:
      expose: false
    input_number.irrigation_cycle1_start_time_sunset_offset:
      expose: false
    input_number.irrigation_cycle2_start_time_sunset_offset:
      expose: false
    sensor.irrigation_cycle1_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle1_start_time_in_seconds:
      expose: false
    sensor.irrigation_cycle1_zone1_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle1_zone2_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle1_zone3_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle1_zone4_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle2_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle2_start_time_in_seconds:
      expose: false
    sensor.irrigation_cycle2_zone1_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle2_zone2_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle2_zone3_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle2_zone4_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle3_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle3_zone1_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle3_zone2_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle3_zone3_actual_duration_in_seconds:
      expose: false
    sensor.irrigation_cycle3_zone4_actual_duration_in_seconds:
      expose: false
    binary_sensor.irrigation_cycle_start_clash:
      expose: false
```

---------------

Simplified, add the data to a separate file and use entity_config: !include_dir_named 

Example:
```
google_assistant:
 project_id: !secret google_assistant_project_id
 secure_devices_pin: !secret google_assistant_secure_devices_pin
 service_account: !include private/google_assistant_report_state_hassio_214617.json
 report_state: true
 entity_config: !include_dir_named google_assistant_entity_config.yaml
```
