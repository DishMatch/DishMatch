DishMatch — Project Spec
App Overview
Description

DishMatch is a mobile-first recipe pairing assistant that helps users quickly decide what to cook by taking an ingredient they have — either a protein or side — and matching it with complementary dishes. The app provides recipe names, images, serving sizes, ingredient lists, and step-by-step instructions.

App Evaluation

Category: Food & Drink / Lifestyle

Mobile: Built for real-time cooking decisions in the kitchen. Optimized for scrolling and recipe detail viewing.

Story: Solves the everyday issue of “I have X… what goes with it?” providing fast, practical cooking inspiration.

Market: Home cooks, college students, beginners, and small households. Niche but widely useful.

Habit: Users consult it when cooking or meal-planning. Moderate habit-building through repeated weekly use.

Scope: Input screen, recipe list (RecyclerView), recipe detail screen. Very doable in course timeline.

Product Spec
1. User Features
Required
-User chooses “Protein” or “Side” mode
-User enters or selects an ingredient
-App fetches recipe pairings (API or JSON)
-RecyclerView displays results (name, image, summary)
-User can tap recipe for full details
-User can save favorites

Stretch Features
-Search filters
-Weekly meal planner
-User-submitted recipes
-AI-pairing suggestions
-Share button
-Swipe gestures
-Push notifications

2. Chosen API(s)
Primary API — Spoonacular Food API
-Recipe titles
-Images
-Summaries
-Ingredient lists
-Yield / serving sizes
-Step-by-step instructions

Used for:
-Listing recipe suggestions
-Populating detail screens
-Searching by ingredient

Backup:
-Static JSON file stored in /assets/recipes.json

3. User Interaction
Required Interactions

User opens app
➜ Shows Protein vs Side menu

User selects mode
➜ Goes to input screen

User enters ingredient + taps “Find Match”
➜ API/JSON returns list → displayed in RecyclerView

User taps recipe
➜ Opens detail screen with ingredients, yield, and steps

User taps ⭐ Save
➜ Saves to Favorites (local storage)

User navigates back
➜ Returns to previous list or home

## Wireframes

Below are the hand-drawn wireframes for the DishMatch app:
<img src="(https://github.com/DishMatch/DishMatch/blob/main/IMG_26B88C9B75BA-1.jpeg)" width="600">
