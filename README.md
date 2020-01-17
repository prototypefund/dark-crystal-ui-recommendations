# UI Recommendations

## Letting the peer choose the threshold and number of shards with sliders

Choosing good values for the number of custodians can be confusing, so its important that the interface encourages good values to be chosen, whilst allowing for some flexibility depending on the individual situation.  We recommend giving feedback similar to how when choosing a password you might receive feedback on how strong it is. 

![Crystal pie 1](./assets/crystalpie1.svg)

With sensible values the indicator stays green.

![Crystal pie 2](./assets/crystalpie2.svg)

With progressively less sensible values the indicator changes colour, indicating either a danger of loss (threshold too high) or insecurity (threshold too low, or number of shares too high).

## Interface in original dark-crystal implementation

Unlike application-specific key backup mechanisms, the original dark-crystal implementation was designed to be a generic tool for backing up any key or secret, so the peer is able to enter the secret itself.

With integrated applications this is not nessecary, which is lucky because the process of copying and pasting keys can be quite cumbersome, error-prone and has security issues. 

![gif](./assets/dark-crystal-3.gif)

Here we see a short demo of entering data and selecting custodians in the original implementation.

![screenshot showing secret history](./assets/secret-history-screenshot.png)

This screenshot shows the history of a secret; who the shards were sent to and buttons to request them back.

## Learnings from original implementation

- [Peer testing and usability assessment](https://gitlab.com/dark-crystal/research/blob/master/dark_crystal-report_peer_testing_and_usability_assessment.md)
- [UX Report from UnderExposed Design Residency with Ura Design - Part1](https://gitlab.com/dark-crystal/research/blob/master/underexposed1.md)
- [UX Report from UnderExposed Design Residency with Ura Design - Part 2](https://gitlab.com/dark-crystal/research/blob/master/underexposed2.md)
