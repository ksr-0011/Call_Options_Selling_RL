# Project 4: Call Options

## Overview

This project involves creating an agent that decides when to exercise a call option within a given time span of \( T \) days. The goal is to maximize the investor's profit from exercising the call option.

## Problem Description

An investor holds a call option to buy one share of a stock at a fixed price \( p \). The investor has \( T \) days to decide whether to exercise the option. The decision is made at the beginning of each day. If the investor exercises the option on a day when the stock price is \( s \), the effective profit is \( (s - p) \).

### Stock Price Dynamics

- The price of the stock varies with independent increments.
- The price on day \( t + 1 \) is given by \( S_{t+1} = S_t + W_t \), where \( \{W_t\}_{t \ge 1} \) is an i.i.d. process.
- The process \( \{W_t\} \) is discretely uniformly distributed with endpoints \( -\epsilon \) and \( +\epsilon \), for some \( \epsilon \in \mathbb{N} \). For example, if \( \epsilon = 5 \), then \( W_t \sim U\{-5, 5\} \).

## Objective

The primary objective is to develop an agent that can decide the optimal day to exercise the call option within the given \( T \) days to maximize the investor's profit.
