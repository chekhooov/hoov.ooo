---
title: 'CS61BYoG, A Random Map Generator'
date: 2022-10-11T12:30:13+08:00
draft: false
---

## Introduction

lorem, die

## Overview

lorem, test

## Code Structure

lorem, test

## Phase 1: World Generation

lorem

```java
public class MapGenerator extends StageBuilder {
		// Fields
    private static final int numRoomTries = 50;
    private static final int extraConnectorChance = 40;
    private static final int roomExtraSize = 0;
    private static final int windingPercent = 60;

		private final int width;
    private final int height;
    private final Random r;

    private TETile[][] _map;
    private List<Room> _rooms;
    private Player _player;
		...

		// Constructors
    public MapGenerator(int width, int height, long seed) {
        this.width = width;
        this.height = height;
        this.r = new Random(seed);
        generate();
    }

		// Methods
		public TETile[][] getMap() { ... }
		public void move(char c) { ... }
		...

		private void generate() { ... }
		private void addRooms() { ... }
		private void growMaze(Position start) { ... }
		private void connectRegions() { ... }
		...
}
```
