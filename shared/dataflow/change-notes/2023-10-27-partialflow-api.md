---
category: fix
---
* The API for debugging flow using partial flow has changed slightly. Instead of using `module Partial = FlowExploration<limit/0>` and choosing between `Partial::partialFlow` and `Partial::partialFlowRev`, you now choose between `module Partial = FlowExplorationFwd<limit/0>` and `module Partial = FlowExplorationRev<limit/0>`, and then always use `Partial::partialFlow`.
