# Repository Instructions

## Terminology

Use these terms consistently in this repository:

| Term | Meaning |
| --- | --- |
| `食材` | Unit of an item when buying, packing, or carrying it, such as rice or salt. |
| `メニュー` | Unit of a dish made from `食材`; the unit people actually eat. |

## Recipe Documentation

When writing or updating a recipe, classify every ingredient into one of these groups:

| Group | Meaning |
| --- | --- |
| `Mandatory` | Ingredients that define the dish and should not be omitted. |
| `Required` | Ingredients needed for the standard version, with substitutions allowed when noted. |
| `Advisary` | Optional ingredients, flavor variations, toppings, or preference-based additions. |

Use these exact group labels in recipe ingredient sections.
If a classification is uncertain, describe it as a guideline or estimate rather than a fixed fact.

## Recipe Equipment Ownership

When adding or updating a recipe, check the required cooking tools listed in the recipe against `data/gear.csv`.
If any required cooking tool does not have an assigned owner, add a task to `tasks/todo.md` to decide who will bring it.

## Avoid Generic Over-Caution

Do not add broad, generic accommodations or preference notes unless they are supported by the repository context or explicitly requested by the user.
For example, avoid LLM-style over-consideration such as "if someone dislikes cilantro" when no such preference is documented.
Only include dietary restrictions, allergies, dislikes, substitutions, or special handling notes when they are relevant to the actual plan.

## Derived Food List

`docs/food-list.md` is derived from the recipes in `docs/recipes/`.
When adding, updating, renaming, or deleting a recipe, update `docs/food-list.md` in the same change so it remains a complete food list.
