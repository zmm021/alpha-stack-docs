# Config Guide

## Overview

所有参数集中在 YAML config 中，按层划分：

-   macro
-   sector
-   symbol
-   signal

------------------------------------------------------------------------

## Symbol Indicators

-   ma_short_window
-   ma_long_window
-   atr_window
-   volume_window
-   high_window_short
-   high_window_mid
-   range_position_window_short
-   range_position_window_mid

------------------------------------------------------------------------

## Signal Config

-   enable_cooldown
-   emit_only_on_switch
-   buy_to_exit_cooldown_hours
-   exit_to_buy_cooldown_hours

Range thresholds: - range_buy_position_threshold -
range_reduce_position_threshold - range_sell_position_threshold

Risk: - exhausted_action - breakdown_action - high_risk_action -
risk_off_action
