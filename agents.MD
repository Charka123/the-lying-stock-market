# Project Overview

## Game Concept
A stock market simulation game developed using Godot.

The player participates in a fictional stock market, buying and
selling shares of different companies to grow their portfolio.

The game revolves around the theme:
"The Best Part of 'Believe' is the Lie."

## Core Theme
The game explores the relationship between market perception
and actual company fundamentals.

Stock prices are influenced by both underlying company performance
and public sentiment. News, rumors, and misleading information
can cause stock prices to deviate significantly from their
fundamental values.

Players must decide whether to trust available information
or take advantage of market expectations.

## Genre
- Simulation
- Strategy
- Management

# Technology Stack

- Game Engine: Godot
- Programming Language: GDScript
- Target Platform: Desktop

## Technical Guidelines
- Use GDScript for gameplay logic.
- Prefer Godot's built-in functionality over external dependencies.
- Use Godot signals for communication between loosely coupled nodes.
- Avoid unnecessary third-party plugins.

# Core Gameplay

## Gameplay Loop
1. The player views the available stocks.
2. The player reviews company information and market news.
3. The player buys or sells shares.
4. The market advances to the next day.
5. Stock prices update based on market conditions.
6. The player evaluates their portfolio.
7. Repeat until the simulation ends.

## Stock Market System

Each company has:
- Company name
- Stock ticker
- Current stock price
- Fundamental value
- Public sentiment
- Volatility
- Available shares (if applicable)

Stock prices are influenced by:
- Company fundamentals
- Public sentiment
- Market news and events
- Random market fluctuations

## Trading System
- Players can buy shares.
- Players can sell shares they own.
- Players must have sufficient cash to buy shares.
- Players cannot sell more shares than they own.
- Transactions update the player's portfolio and cash balance.

## Simulation Time
- The simulation progresses in daily turns.
- The player can advance the simulation by one day.
- Market events and stock prices update when a new day begins.

# Architecture Guidelines

- Keep market simulation logic separate from UI logic.
- Keep portfolio management separate from stock price calculations.
- Use Resources or other appropriate data structures for company
  and stock definitions.
- Avoid putting all game logic into a single script.
- Use signals for communication between independent systems.
- Use Autoloads only for systems that genuinely require global access.
- Avoid unnecessary coupling between scenes.