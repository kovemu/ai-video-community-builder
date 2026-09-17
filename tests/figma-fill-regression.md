# Figma auto-layout FILL regression

Reproduction from Figma Desktop:

`in set_layoutSizingHorizontal: FILL can only be set on children of auto-layout frames`

Root cause: `Home Composer.layoutSizingHorizontal = 'FILL'` was assigned before `Home Composer` had been appended to the auto-layout `Home Feed` parent.

Regression requirement: any `layoutSizingHorizontal = 'FILL'` or `layoutSizingVertical = 'FILL'` assignment must happen only after the node is attached to an auto-layout parent.

Local automated test: `Home build only sets FILL after the node has an auto-layout parent` using a strict Figma mock that throws the same error.
