// ███╗   ██╗ ██████╗     ████████╗ ██████╗ ██╗   ██╗ ██████╗██╗  ██╗██╗██╗██╗
// ████╗  ██║██╔═══██╗    ╚══██╔══╝██╔═══██╗██║   ██║██╔════╝██║  ██║██║██║██║
// ██╔██╗ ██║██║   ██║       ██║   ██║   ██║██║   ██║██║     ███████║██║██║██║
// ██║╚██╗██║██║   ██║       ██║   ██║   ██║██║   ██║██║     ██╔══██║╚═╝╚═╝╚═╝
// ██║ ╚████║╚██████╔╝       ██║   ╚██████╔╝╚██████╔╝╚██████╗██║  ██║██╗██╗██╗
// ╚═╝  ╚═══╝ ╚═════╝        ╚═╝    ╚═════╝  ╚═════╝  ╚═════╝╚═╝  ╚═╝╚═╝╚═╝╚═╝
{
  "id": "overgrowntemple",
  "resource-packs": [
    "OvergrownTemple"
  ],
  "object-groups": [
    "overgrowntemple/objectgroup",
    "sub_steamchamber/objectgroup",
    "sub_spidernest/objectgroup",
    "sub_boobytrap/objectgroup",
    "sub_troom/objectgroup",
    "sub_treasureroom/objectgroup",
    "sub_templetunnel/objectgroup"
  ],
  "loctable-id": "overgrowntempleLoctable",
  "require-matching-doors": true,
  "default-mobs": {
    "only": [
      "jungle-mix"
    ],
    "density": 1
  },
  "rules": {
    "modifiers": [
      {
        "properties": {
          "NightMode": "1"
        }
      },
      {
        "properties": {
          "PlayerDamage": "0.5"
        }
      },
      {
        "properties": {
          "MobHealth": "1.0"
        }
      }
    ],
    "tiles": [
      {
        "id": "steam_room",
        "challenges": [
          "steam_room_arena"
        ],
        "rotations": [
          0
        ],
        "teleports": [
          {
            "door": "steam_door",
            "exit": "*.ot_temple_arena.travel_steam",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "nest_1",
        "rotations": [
          90
        ],
        "teleports": [
          {
            "door": "spider_door",
            "exit": "*.ot_temple_sidepath_spider.travel_spider",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "nest_3",
        "challenges": [
          "miniarena"
        ]
      },
      {
        "id": "trap_1",
        "rotations": 180,
        "challenges": [
          "booby_endend_arena"
        ],
        "teleports": [
          {
            "door": "trap_door",
            "exit": "*.ot_temple_jungle_04.travel_booby",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          },
          {
            "door": "end_door2",
            "exit": "*.trap_6.end_door1",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "trap_2",
        "entry-door": "enter"
      },
      {
        "id": "trap_3",
        "entry-door": "enter1"
      },
      {
        "id": "trap_4",
        "entry-door": "enter2"
      },
      {
        "id": "trap_5",
        "entry-door": "enter3"
      },
      {
        "id": "trap_6",
        "challenges": [
          "booby_end_arena"
        ],
        "teleports": [
          {
            "door": "end_door1",
            "exit": "*.trap_1.end_door2",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "troom_stretch",
        "rotations": 270,
        "teleports": [
          {
            "door": "troom_door",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          },
          {
            "door": "troom_exit_1",
            "exit": "*.troom_end.troom_exit_2",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_cave"
          }
        ]
      },
      {
        "id": "troom_middle",
        "challenges": [
          "troom_mid_arena1"
        ]
      },
      {
        "id": "troom_middle_1",
        "challenges": [
          "troom_clicky",
          "troom_mid_arena"
        ]
      },
      {
        "id": "troom_end",
        "challenges": [
          "troom_end_arena"
        ],
        "teleports": [
          {
            "door": "troom_exit_2",
            "exit": "*.troom_stretch.troom_end_1",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_cave"
          }
        ]
      },
      {
        "id": "treasure_stairs",
        "rotations": [
          90
        ],
        "challenges": [
          "treasure_backtrack_2"
        ],
        "teleports": [
          {
            "door": "flooded_door",
            "exit": "*.ot_temple_sidepath_flooded.travel_flooded",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "treasure_path",
        "rotations": [
          90
        ],
        "entry-door": "enter",
        "challenges": [
          "treasure_backtrack"
        ]
      },
      {
        "id": "treasure_room",
        "rotations": [
          90
        ],
        "challenges": [
          "treasure_arena1"
        ]
      },
      {
        "id": "tun_start",
        "rotations": [
          180
        ],
        "teleports": [
          {
            "door": "tunnel_door",
            "exit": "*.ot_temple_sidepath_tunnel.travel_tunnel",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "tun_mid_2",
        "rotations": [
          180,
          270
        ]
      },
      {
        "id": "tun_mid_3",
        "challenges": [
          "tunnel_clicky_arena"
        ]
      },
      {
        "id": "tun_hall",
        "challenges": [
          "tunnel_arena_hall"
        ]
      },
      {
        "id": "tun_mid_1",
        "entry-door": "enter",
        "exit-door": "exit"
      },
      {
        "id": "tun_mid_4",
        "entry-door": "enter"
      },
      {
        "id": "tun_mid_5",
        "challenges": [
          "skeleton_arena"
        ],
        "entry-door": "enter"
      },
      {
        "id": "tun_mid_6",
        "entry-door": "enter"
      },
      {
        "id": "tun_right_1",
        "rotations": [
          90
        ],
        "entry-door": "enter"
      },
      {
        "id": "tun_right_2",
        "rotations": [
          90
        ],
        "entry-door": "enter",
        "challenges": [
          "tunnel_clicky_arena1"
        ]
      },
      {
        "id": "tun_end",
        "challenges": [
          "tunnel_end_arena"
        ],
        "teleports": [
          {
            "door": "tunnel_exit_door",
            "exit": "*.ot_temple_09.travel_tunnel_exit",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_start_new",
        "rotations": 0
      },
      {
        "id": "ot_jungle_edge_01",
        "entry-door": "enter"
      },
      {
        "id": "ot_jungle_edge_02"
      },
      {
        "id": "ot_temple_entrance",
        "rotations": 270,
        "entry-door": "enter_001"
      },
      {
        "id": "ot_entrance_hall",
        "entry-door": "entrance_hall_01",
        "exit-door": "entrance_hall_02"
      },
      {
        "id": "ot_entrance_hall_alt",
        "entry-door": "entrance_hall_01",
        "exit-door": "entrance_hall_02"
      },
      {
        "id": "ot_temple_01",
        "rotations": [
          90,
          180
        ]
      },
      {
        "id": "ot_temple_arena",
        "entry-door": "enter_002",
        "rotations": 90,
        "teleports": [
          {
            "door": "travel_steam",
            "exit": "steam_door",
            "dungeons": [
              "sub_steamchamber"
            ],
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_temple_arena_alt",
        "entry-door": "enter_002_alt",
        "rotations": 90
      },
      {
        "id": "ot_temple_jungle_01",
        "entry-door": "enter_003",
        "rotations": 0
      },
      {
        "id": "ot_temple_jungle_02",
        "entry-door": "enter_004"
      },
      {
        "id": "ot_temple_jungle_03",
        "entry-door": "enter_005"
      },
      {
        "id": "ot_temple_jungle_04",
        "entry-door": "enter_006",
        "teleports": [
          {
            "door": "travel_booby",
            "exit": "trap_door",
            "dungeons": [
              "sub_boobytrap"
            ],
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_temple_jungle_04_alt",
        "entry-door": "enter_006_alt"
      },
      {
        "id": "ot_temple_boss_gate",
        "entry-door": "enter_007",
        "exit-door": "bossgate_exit",
        "rotations": 90,
        "teleports": [
          {
            "door": "travel_treasue",
            "exit": "troom_door",
            "dungeons": [
              "sub_troom"
            ],
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Temple"
          }
        ]
      },
      {
        "id": "ot_temple_boss_stairs_01",
        "entry-door": "enter_008",
        "challenges": [
          "ot_stairs_arena_01"
        ]
      },
      {
        "id": "ot_temple_boss_stairs_02_new",
        "entry-door": "enter_009_2",
        "challenges": [
          "ot_stairs_arena_02"
        ]
      },
      {
        "id": "ot_boss_arena_new",
        "entry-door": "enter_010_2"
      },
      {
        "id": "ot_temple_exit_01",
        "entry-door": "enter_011"
      },
      {
        "id": "ot_temple_sidepath_spider",
        "rotations": 270,
        "teleports": [
          {
            "door": "travel_spider",
            "exit": "spider_door",
            "dungeons": [
              "sub_spidernest"
            ],
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_temple_sidepath_flooded",
        "rotations": [
          180,
          270
        ],
        "teleports": [
          {
            "door": "travel_flooded",
            "exit": "flooded_door",
            "dungeons": [
              "sub_floodtemp"
            ],
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_temple_sidepath_flooded_alt",
        "rotations": [
          180,
          270
        ]
      },
      {
        "id": "ot_temple_sidepath_tunnel",
        "rotations": [
          180,
          270
        ],
        "teleports": [
          {
            "door": "travel_tunnel",
            "exit": "tunnel_door",
            "dungeons": [
              "sub_templetunnel"
            ],
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_temple_09",
        "rotations": 90,
        "entry-door": "enter_012",
        "teleports": [
          {
            "door": "travel_tunnel_exit",
            "object": "Decor/Prefabs/DoorTravel/BambooBluff/BP_TravelDoor_Cave"
          }
        ]
      },
      {
        "id": "ot_jungle_deadend_02",
        "challenges": [
          "jungle_deadend_trap"
        ]
      },
      {
        "id": "ot_temple_deadend_02",
        "challenges": [
          "temple_deadend_trap_02"
        ]
      },
      {
        "id": "ot_temple_deadend_05",
        "challenges": [
          "temple_deadend_trap_05"
        ]
      },
      {
        "id": "ot_temple_deadend_06",
        "challenges": [
          "temple_deadend_trap_06"
        ]
      },
      {
        "id": "ot_temple_deadend_loot",
        "challenges": [
          "temple_deadend_trap_loot"
        ]
      },
      {
        "id": "ot_temple_deadend_goldkey_01",
        "challenges": [
          "goldkey_battle_left"
        ],
        "rotations": [
          90
        ]
      },
      {
        "id": "ot_temple_deadend_goldkey_02",
        "challenges": [
          "goldkey_battle_right"
        ],
        "rotations": [
          90
        ]
      }
    ],
    "stretches": [
      {
        "tiles": [
          "ot_start_new"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix-pass"
          ]
        }
      },
      {
        "tiles": [
          "ot_jungle_edge_01",
          "ot_jungle_edge_02"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_jungle_deadend_01",
          "ot_jungle_deadend_02",
          {
            "id": "ot_jungle_deadend_cap_01",
            "weight": 0.2
          },
          {
            "id": "ot_jungle_deadend_cap_02",
            "weight": 0.1
          }
        ],
        "side-paths": {
          "probability": 1,
          "default": {
            "max-length": [
              1,
              1
            ],
            "dead-ends": [
              "ot_jungle_deadend_01",
              "ot_jungle_deadend_02",
              {
                "id": "ot_jungle_deadend_cap_01",
                "weight": 0.02
              },
              {
                "id": "ot_jungle_deadend_cap_02",
                "weight": 0.01
              }
            ],
            "tile-groups": [
              "jungle_sidepath"
            ]
          }
        }
      },
      {
        "tiles": [
          "ot_temple_entrance"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "id": "entrance_hall",
        "tiles": [
          "ot_entrance_hall",
          "ot_entrance_hall_alt"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "length": 1,
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.02
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.01
          }
        ],
        "side-paths": {
          "probability": 1,
          "default": {
            "max-length": [
              1,
              1
            ],
            "dead-ends": [
              {
                "id": "ot_temple_sidepath_tunnel",
                "weight": 0.45
              },
              {
                "id": "ot_temple_sidepath_flooded",
                "weight": 0.4
              },
              {
                "id": "ot_temple_sidepath_flooded_alt",
                "weight": 0.15
              }
            ],
            "tile-groups": [
              "templeentrance_sidepath_01",
              "templeentrance_sidepath_02"
            ]
          }
        }
      },
      {
        "id": "temple_run_1",
        "tiles": [
          "ot_temple_01",
          "ot_temple_02",
          "ot_temple_03",
          "ot_temple_04",
          "ot_temple_05",
          "ot_temple_06",
          "ot_temple_07",
          "ot_temple_08"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "id": "temple_sidepath_1",
        "tiles": [
          "ot_temple_multi_01",
          "ot_temple_multi_02",
          "ot_temple_multi_03"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.02
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.01
          }
        ],
        "side-paths": {
          "probability": 1,
          "default": {
            "max-length": [
              1,
              1
            ],
            "dead-ends": [
              {
                "id": "ot_temple_sidepath_spider",
                "weight": 0.85
              },
              {
                "id": "ot_temple_deadend_02",
                "weight": 0.15
              }
            ],
            "tile-groups": [
              "templespider_sidepath"
            ]
          }
        }
      },
      {
        "id": "temple_run_2",
        "tiles": [
          "ot_temple_01",
          "ot_temple_02",
          "ot_temple_03",
          "ot_temple_04",
          "ot_temple_05",
          "ot_temple_06",
          "ot_temple_07",
          "ot_temple_08"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "id": "temple_sidepath_2",
        "tiles": [
          "ot_temple_multi_01",
          "ot_temple_multi_02",
          "ot_temple_multi_03"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.02
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.01
          }
        ]
      },
      {
        "id": "tunnel_exit",
        "tiles": [
          "ot_temple_09"
        ]
      },
      {
        "id": "temple_arena",
        "tiles": [
          {
            "id": "ot_temple_arena",
            "weight": 0.32
          },
          {
            "id": "ot_temple_arena_alt",
            "weight": 0.68
          }
        ]
      },
      {
        "id": "temple_sidepath_3",
        "tiles": [
          "ot_temple_multi_01",
          "ot_temple_multi_02",
          "ot_temple_multi_03"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.02
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.01
          }
        ]
      },
      {
        "id": "temple_run_4",
        "tiles": [
          "ot_temple_01",
          "ot_temple_02",
          "ot_temple_03",
          "ot_temple_04",
          "ot_temple_05",
          "ot_temple_06"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "id": "temple_sidepath_4",
        "tiles": [
          "ot_temple_multi_01",
          "ot_temple_multi_02",
          "ot_temple_multi_03"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.2
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.1
          }
        ],
        "side-paths": {
          "probability": 1,
          "default": {
            "max-length": [
              1,
              1
            ],
            "dead-ends": [
              "ot_temple_deadend_01",
              "ot_temple_deadend_02",
              "ot_temple_deadend_03",
              "ot_temple_deadend_04",
              "ot_temple_deadend_05",
              "ot_temple_deadend_06",
              "ot_temple_deadend_07",
              "ot_temple_deadend_08",
              "ot_temple_deadend_loot",
              {
                "id": "ot_deadend_cap_01",
                "weight": 0.02
              },
              {
                "id": "ot_deadend_cap_02",
                "weight": 0.01
              }
            ],
            "tile-groups": [
              "templegeneric_sidepath"
            ]
          }
        }
      },
      {
        "tiles": [
          "ot_temple_jungle_01"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "tiles": [
          "ot_temple_jungle_02"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "tiles": [
          "ot_temple_jungle_03"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "tiles": [
          {
            "id": "ot_temple_jungle_04",
            "weight": 0.3
          },
          {
            "id": "ot_temple_jungle_04_alt",
            "weight": 0.7
          }
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "id": "temple_sidepath_5",
        "tiles": [
          "ot_temple_multi_01",
          "ot_temple_multi_02",
          "ot_temple_multi_03"
        ],
        "length": 1,
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.02
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.01
          }
        ]
      },
      {
        "id": "temple_boss_gate",
        "tiles": [
          "ot_temple_boss_gate"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        },
        "dead-ends": [
          "ot_temple_deadend_01",
          "ot_temple_deadend_02",
          "ot_temple_deadend_03",
          "ot_temple_deadend_04",
          "ot_temple_deadend_05",
          "ot_temple_deadend_06",
          "ot_temple_deadend_07",
          "ot_temple_deadend_08",
          "ot_temple_deadend_loot",
          {
            "id": "ot_deadend_cap_01",
            "weight": 0.02
          },
          {
            "id": "ot_deadend_cap_02",
            "weight": 0.01
          }
        ],
        "side-paths": {
          "probability": 1,
          "default": {
            "max-length": [
              1,
              1
            ],
            "dead-ends": [
              "ot_temple_deadend_goldkey_02"
            ],
            "tile-groups": [
              "templebossgate_sidepath"
            ]
          }
        }
      },
      {
        "tiles": [
          "ot_temple_boss_stairs_01"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "tiles": [
          "ot_temple_boss_stairs_02_new"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "id": "big_fight",
        "tiles": [
          "ot_boss_arena_new"
        ]
      },
      {
        "tiles": [
          "ot_temple_exit_01"
        ],
        "mobs": {
          "density": 1,
          "only": [
            "jungle-mix"
          ]
        }
      },
      {
        "tiles": [
          "ot_temple_exit_02"
        ],
        "mobs": {
          "density": 1.5,
          "only": [
            "jungle-mix"
          ]
        }
      }
    ],
    "tile-groups": [
      {
        "#": "jungle_sidepath",
        "id": "jungle_sidepath",
        "tiles": [
          "ot_jungle_sidepath_01",
          "ot_jungle_sidepath_02"
        ]
      },
      {
        "#": "templeentrance_sidepath_01",
        "id": "templeentrance_sidepath_01",
        "tiles": [
          "ot_temple_sidepath_02",
          "ot_temple_sidepath_03",
          "ot_temple_sidepath_05"
        ]
      },
      {
        "#": "templeentrance_sidepath_02",
        "id": "templeentrance_sidepath_02",
        "tiles": [
          "ot_temple_sidepath_01",
          "ot_temple_sidepath_04",
          "ot_temple_sidepath_06"
        ]
      },
      {
        "#": "templegeneric_sidepath",
        "id": "templegeneric_sidepath",
        "tiles": [
          {
            "id": "ot_temple_sidepath_01",
            "weight": 0.2
          },
          {
            "id": "ot_temple_sidepath_02",
            "weight": 0.1
          },
          {
            "id": "ot_temple_sidepath_03",
            "weight": 0.2
          },
          {
            "id": "ot_temple_sidepath_04",
            "weight": 0.1
          },
          {
            "id": "ot_temple_sidepath_05",
            "weight": 0.3
          },
          {
            "id": "ot_temple_sidepath_06",
            "weight": 0.2
          }
        ]
      },
      {
        "#": "templespider_sidepath",
        "id": "templespider_sidepath",
        "tiles": [
          {
            "id": "ot_temple_sidepath_01",
            "weight": 0.3
          },
          {
            "id": "ot_temple_sidepath_02",
            "weight": 0.3
          },
          {
            "id": "ot_temple_sidepath_03",
            "weight": 0.2
          },
          {
            "id": "ot_temple_sidepath_05",
            "weight": 0.1
          },
          {
            "id": "ot_temple_sidepath_06",
            "weight": 0.1
          }
        ]
      },
      {
        "#": "templebossgate_sidepath",
        "id": "templebossgate_sidepath",
        "tiles": [
          "ot_temple_deadend_goldkey_01"
        ]
      }
    ],
    "objectives": [
      {
        "name": "name_ot_01",
        "description": "description_ot_g_01",
        "displayMode": "MainObjective",
        "gauntlet": {
          "end-region": "*.ot_temple_entrance.obj_find_temple"
        }
      },
      {
        "name": "name_ot_01",
        "description": "description_ot_c_01",
        "displayMode": "MainObjective",
        "gauntlet": {
          "end-region": "entrance_hall.*.obj_enter_temple"
        }
      },
      {
        "name": "name_ot_01",
        "description": "description_ot_g_03",
        "displayMode": "MainObjective",
        "gauntlet": {
          "end-region": "temple_arena.*.obj_reach_arena"
        }
      },
      {
        "name": "name_ot_01",
        "description": "description_ot_c_02",
        "displayMode": "MainObjective",
        "click": {
          "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Ruby/BP_Ruby",
          "count": 1,
          "locations": [
            "temple_arena.*.obj_arena_switch"
          ],
          "locked-doors": [
            "temple_arena.*.obj_arena_gate"
          ],
          "door-path": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_9x"
        }
      },
      {
        "name": "name_ot_01",
        "description": "description_ot_a_01",
        "displayMode": "MainObjective",
        "arena": {
          "stretch": "temple_arena",
          "start-time": 1,
          "interval": 25,
          "rest-interval": 0.5,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              6,
              "arena-mix"
            ],
            [
              8,
              "arena-mix"
            ],
            [
              2,
              "arena-leaper"
            ],
            [
              10,
              "arena-mix"
            ],
            [
              10,
              "arena-mix"
            ],
            [
              3,
              "arena-leaper"
            ],
            [
              6,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_9x",
            "start-unlocked": false
          }
        }
      },
      {
        "name": "name_ot_01",
        "description": "description_ot_g_04",
        "displayMode": "MainObjective",
        "gauntlet": {
          "end-region": "*.ot_temple_boss_gate.obj_reach_boss_gate"
        }
      },
      {
        "name": "name_ot_01",
        "description": "description_ot_k_01",
        "displayMode": "MainObjective",
        "consider-tiles": "all",
        "click": {
          "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_DoorLocked_Gold_OvergrownTemple",
          "count": 1,
          "locations": [
            "*.*.obj_boss_gate_silvergate"
          ],
          "key-locations": [
            "*.*.obj_boss_gate_key"
          ],
          "key-type": "gold",
          "mobs": [
            25,
            "arena-mix"
          ],
          "spawn-regions": [
            "*.*.bad_boys"
          ]
        }
      },
      {
        "name": "name_ot_02",
        "description": "description_ot_g_05",
        "displayMode": "MainObjective",
        "gauntlet": {
          "end-region": "big_fight.*.obj_reach_boss"
        }
      },
      {
        "name": "name_ot_02",
        "description": "description_ot_b_01",
        "displayMode": "MainObjective",
        "arena": {
          "stretch": "big_fight",
          "interval": 30,
          "rest-interval": 5,
          "start-time": 2,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "is-boss": true,
          "waves": [
            [
              1,
              "jungleabomination"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_JungleDoorDown_5",
            "start-unlocked": false
          }
        }
      },
      {
        "name": "name_ot_03",
        "description": "description_ot_g_06",
        "displayMode": "MainObjective",
        "gauntlet": {
          "end-region": "*.ot_temple_exit_02.obj_reach_exit"
        }
      },
      {
        "name": "name_ot_03",
        "description": "description_ot_g_07",
        "displayMode": "MainObjective",
        "click": {
          "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_Door7x4",
          "count": 1,
          "locations": [
            "*.ot_temple_exit_02.obj_temple_exit"
          ]
        }
      }
    ],
    "challenges": [
      {
        "id": "steam_room_arena",
        "trigger": "*.*.steam_arena",
        "reward": {
          "region": "*.steam_room.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 20,
          "rest-interval": 0.5,
          "start-time": 2,
          "prespawn-mob": "",
          "waves": [
            [
              15,
              "arena-mix"
            ],
            [
              15,
              "arena-mix"
            ],
            [
              15,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "miniarena",
        "trigger": "*.*.obj_surprise_spiders",
        "reward": {
          "region": "*.*.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 6,
          "rest-interval": 0,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              12,
              "spidernest"
            ],
            [
              10,
              "spidernest"
            ],
            [
              8,
              "spidernest"
            ],
            [
              11,
              "spidernest"
            ],
            [
              13,
              "spidernest"
            ],
            [
              8,
              "spidernest"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_gate_bb_bamboo_x5",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "booby_endend_arena",
        "trigger": "*.*.arena_trigger",
        "reward": {
          "region": "*.trap_1.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 30,
          "rest-interval": 0.5,
          "start-time": 45,
          "prespawn-mob": "",
          "waves": [
            [
              15,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "booby_end_arena",
        "trigger": "*.*.arena_trigger",
        "reward": {
          "region": "*.trap_6.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 30,
          "rest-interval": 0.5,
          "start-time": 0,
          "prespawn-mob": "",
          "waves": [
            [
              10,
              "arena-mix"
            ],
            [
              12,
              "arena-mix"
            ],
            [
              8,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_Gate_BB_Bamboo_x5",
            "start-unlocked": false
          }
        }
      },
      {
        "id": "troom_clicky",
        "trigger": "*.troom_middle_1.click_trigger",
        "click": {
          "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_Button_Temple",
          "door-path": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_TempleDoorDown_5",
          "count": 4,
          "locations": [
            "*.troom_middle_1.beacon"
          ],
          "locked-doors": [
            "*.troom_middle_1.gate1"
          ]
        }
      },
      {
        "id": "troom_mid_arena1",
        "trigger": "*.*.troom_arena_trigger",
        "reward": {
          "region": "*.troom_middle.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 10,
          "rest-interval": 0,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              5,
              "arena-mix"
            ],
            [
              10,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "troom_mid_arena",
        "trigger-object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_Bamboo_Cog",
        "reward": {
          "region": "*.troom_middle_1.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 10,
          "rest-interval": 0,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              20,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_gate_bb_bamboo_x5",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "troom_end_arena",
        "trigger": "*.*.troom_trigger",
        "reward": {
          "region": "*.troom_end.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 20,
          "rest-interval": 2,
          "start-time": 0.5,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              5,
              "arena-mix"
            ],
            [
              3,
              "arena-leaper"
            ],
            [
              10,
              "arena-mix"
            ],
            [
              3,
              "arena-leaper"
            ],
            [
              8,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_TempleDoorDown_5",
            "start-unlocked": false
          }
        }
      },
      {
        "id": "treasure_arena1",
        "trigger": "*.*.flooded_arena",
        "reward": {
          "region": "*.treasure_room.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_woodenchest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 8,
          "rest-interval": 1,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              6,
              "arena-mix"
            ],
            [
              6,
              "arena-mix"
            ],
            [
              3,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "treasure_backtrack",
        "trigger": "*.*.backtrack_arena_trigger",
        "arena": {
          "stretch": "",
          "interval": 0,
          "rest-interval": 2,
          "start-time": 30,
          "prespawn-mob": "",
          "waves": [
            [
              10,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "treasure_backtrack_2",
        "trigger": "*.*.backtrack_arena_trigger_2",
        "arena": {
          "stretch": "",
          "interval": 0,
          "rest-interval": 2,
          "start-time": 30,
          "prespawn-mob": "",
          "waves": [
            [
              10,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "tunnel_clicky_arena",
        "trigger": "*.*.tun_arena_trigger",
        "reward": {
          "region": "*.tun_mid_3.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 30,
          "rest-interval": 0,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              16,
              "arena-mix"
            ],
            [
              22,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "tunnel_arena_hall",
        "trigger": "*.*.tun_hall_trigger",
        "reward": {
          "region": "*.tun_hall.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 30,
          "rest-interval": 0.5,
          "start-time": 2,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              15,
              "arena-mix"
            ],
            [
              10,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "skeleton_arena",
        "trigger-object": "Decor/Prefabs/Skeleton/BP_Crypt_Skeleton_Clicky",
        "reward": {
          "region": "*.*.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "interval": 5,
          "rest-interval": 0,
          "start-time": 0,
          "waves": [
            [
              5,
              "skeleton-mix-easy"
            ],
            [
              6,
              "skeleton-mix-easy"
            ],
            [
              4,
              "skeleton-mix-easy"
            ],
            [
              10,
              "skeleton-mix-easy"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "tunnel_clicky_arena1",
        "trigger-object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Ruby/BP_Sapphire",
        "reward": {
          "region": "*.tun_right_2.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 10,
          "rest-interval": 0,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              22,
              "arena-mix"
            ],
            [
              8,
              "arena-mix"
            ],
            [
              6,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "tunnel_end_arena",
        "trigger": "*.*.end_trigger",
        "reward": {
          "region": "*.tun_end.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "",
          "interval": 0,
          "rest-interval": 0,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              20,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/BP_Gate_BB_Bamboo_x5",
            "start-unlocked": false
          }
        }
      },
      {
        "id": "ot_stairs_arena_01",
        "trigger": "*.*.obj_stair_challenge",
        "reward": {
          "region": "*.*.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 3,
          "rest-interval": 1,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              1,
              "creeper-mix"
            ],
            [
              2,
              "creeper-mix"
            ],
            [
              3,
              "creeper-mix"
            ],
            [
              3,
              "creeper-mix"
            ],
            [
              2,
              "creeper-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "ot_stairs_arena_02",
        "trigger": "*.*.obj_stair_challenge_redux",
        "reward": {
          "region": "*.*.challengeloot",
          "object": "Decor/Prefabs/RewardChest/BP_FancyChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 3,
          "rest-interval": 1,
          "start-time": 0,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              2,
              "creeper-mix"
            ],
            [
              3,
              "creeper-mix"
            ],
            [
              4,
              "creeper-mix"
            ],
            [
              4,
              "creeper-mix"
            ],
            [
              3,
              "creeper-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_9x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "temple_deadend_trap_02",
        "trigger": "*.ot_temple_deadend_02.trap_trigger",
        "reward": {
          "region": "*.ot_temple_deadend_02.challengereward",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 3,
          "rest-interval": 0,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "temple_deadend_trap_05",
        "trigger": "*.ot_temple_deadend_05.trap_trigger",
        "reward": {
          "region": "*.ot_temple_deadend_05.challengereward",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 4,
          "rest-interval": 0,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "temple_deadend_trap_06",
        "trigger": "*.ot_temple_deadend_06.trap_trigger",
        "reward": {
          "region": "*.ot_temple_deadend_06.challengereward",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 10,
          "rest-interval": 0,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              6,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ],
            [
              8,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "temple_deadend_trap_loot",
        "trigger": "*.ot_temple_deadend_loot.trap_trigger",
        "reward": {
          "region": "*.ot_temple_deadend_loot.challengereward",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 5,
          "rest-interval": 0,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              1,
              "creeper-mix"
            ],
            [
              1,
              "creeper-mix"
            ],
            [
              2,
              "creeper-mix"
            ],
            [
              2,
              "creeper-mix"
            ],
            [
              1,
              "creeper-mix"
            ],
            [
              2,
              "creeper-mix"
            ],
            [
              1,
              "creeper-mix"
            ],
            [
              3,
              "creeper-mix"
            ],
            [
              6,
              "creeper-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "jungle_deadend_trap",
        "trigger": "*.ot_jungle_deadend_02.jungle_trap_trigger",
        "reward": {
          "region": "*.ot_jungle_deadend_02.challengereward",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 10,
          "rest-interval": 1,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              3,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ],
            [
              8,
              "arena-mix"
            ],
            [
              3,
              "arena-mix"
            ]
          ],
          "gate": null
        }
      },
      {
        "id": "goldkey_battle_left",
        "trigger": "*.ot_temple_deadend_goldkey_01.key_trap_left",
        "reward": {
          "region": "*.ot_temple_deadend_goldkey_01.challengereward_left",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 10,
          "rest-interval": 0,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              4,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              4,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              5,
              "arena-mix"
            ],
            [
              8,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      },
      {
        "id": "goldkey_battle_right",
        "trigger": "*.ot_temple_deadend_goldkey_02.key_trap_right",
        "reward": {
          "region": "*.ot_temple_deadend_goldkey_02.challengereward_right",
          "object": "Decor/Prefabs/RewardChest/BP_WoodenChest_Reward"
        },
        "arena": {
          "stretch": "*",
          "interval": 10,
          "rest-interval": 0,
          "start-time": 1,
          "prespawn-mob": "/Game/Actors/Jungle/BP_Jungle_ArenaBattle",
          "waves": [
            [
              1,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              2,
              "arena-mix"
            ],
            [
              1,
              "arena-mix"
            ],
            [
              3,
              "arena-mix"
            ],
            [
              6,
              "arena-mix"
            ]
          ],
          "gate": {
            "object": "Decor/Prefabs/DingyJungle/Jungle_DesignAssets/Overgrown_Temple/BP_OT_Door_5x",
            "start-unlocked": true
          }
        }
      }
    ],
    "mob-groups": [
      {
        "#": "============== JUNGLE MIX PASSIVE ==============",
        "id": "jungle-mix-pass",
        "types": [
          {
            "type": "ocelot",
            "weight": 1
          }
        ],
        "pick-types": [
          1,
          1
        ]
      },
      {
        "#": "============== JUNGLE MIX ==============",
        "id": "jungle-mix",
        "types": [
          {
            "type": "JungleAnimal",
            "weight": 1,
            "max%": 0.05
          },
          {
            "type": "Leaper",
            "weight": 2,
            "max%": 0.1
          },
          {
            "type": "Whisperer",
            "weight": 2,
            "max%": 0.1
          },
          {
            "type": "zombie",
            "weight": 3
          },
          {
            "type": "junglezombie",
            "weight": 7
          },
          {
            "type": "skeleton",
            "weight": 3
          },
          {
            "type": "mossyskeleton",
            "weight": 7
          },
          {
            "type": "skeletonvanguard",
            "weight": 2,
            "max%": 0.3
          },
          {
            "type": "SlimeLarge",
            "weight": 5
          },
          {
            "type": "spider",
            "weight": 2,
            "max%": 0.2
          },
          {
            "type": "creeper",
            "weight": 2,
            "max%": 0.3
          }
        ],
        "pick-types": [
          3,
          5
        ]
      },
      {
        "#": "============== ARENA MIX==============",
        "id": "arena-mix",
        "types": [
          {
            "type": "Leaper",
            "weight": 2,
            "max%": 0.1
          },
          {
            "type": "Whisperer",
            "weight": 2,
            "max%": 0.1
          },
          {
            "type": "zombie",
            "weight": 3
          },
          {
            "type": "junglezombie",
            "weight": 7
          },
          {
            "type": "skeleton",
            "weight": 3
          },
          {
            "type": "mossyskeleton",
            "weight": 7
          },
          {
            "type": "skeletonvanguard",
            "weight": 2,
            "max%": 0.3
          },
          {
            "type": "SlimeLarge",
            "weight": 5
          },
          {
            "type": "spider",
            "weight": 2,
            "max%": 0.2
          },
          {
            "type": "creeper",
            "weight": 2,
            "max%": 0.3
          }
        ],
        "pick-types": [
          3,
          4
        ]
      },
      {
        "#": "============== ARENA LEAPERS ==============",
        "id": "arena-leaper",
        "types": [
          {
            "type": "Leaper",
            "weight": 10
          }
        ],
        "pick-types": [
          1,
          1
        ]
      },
      {
        "#": "============== ENDERMAN ==============",
        "id": "Enderman-solo",
        "types": [
          {
            "type": "Enderman",
            "weight": 10
          }
        ],
        "pick-types": [
          1,
          1
        ]
      },
      {
        "#": "============== CREEPER CHALLENGE MIX ==============",
        "id": "creeper-mix",
        "types": [
          {
            "type": "creeper",
            "weight": 10,
            "max%": 1
          }
        ],
        "pick-types": [
          1,
          1
        ]
      },
      {
        "#": "============== SKELETON MIX EASY ==============",
        "id": "skeleton-mix-easy",
        "types": [
          {
            "type": "skeleton",
            "weight": 8
          },
          {
            "type": "mossyskeleton",
            "weight": 4
          },
          {
            "type": "skeletonvanguard",
            "weight": 2,
            "max%": 0.3
          }
        ],
        "pick-types": [
          2,
          3
        ]
      },
      {
        "#": "============== SPIDERNEST SPECIAL ==============",
        "id": "spidernest-special",
        "types": [
          {
            "type": "cavespider",
            "weight": 10,
            "min": 5
          }
        ]
      },
      {
        "#": "============== SPIDERNEST ==============",
        "id": "spidernest",
        "types": [
          {
            "type": "spider",
            "weight": 2
          },
          {
            "type": "cavespider",
            "weight": 8
          }
        ]
      },
      {
        "#": "============== JUNGLE ABOMINATION ==============",
        "id": "jungleabomination",
        "types": [
          {
            "type": "jungleabomination",
            "min": 1,
            "max": 1
          }
        ]
      }
    ],
    "props": [],
    "prop-groups": [
      {
        "id": "pillar",
        "props": [
          {
            "id": "pillar1",
            "weight": 1
          },
          {
            "id": "pillar2",
            "weight": 1
          },
          {
            "id": "pliiar1",
            "weight": 1
          },
          {
            "id": "pillar2",
            "weight": 1
          }
        ]
      },
      {
        "id": "pole",
        "props": [
          {
            "id": "pole1",
            "weight": 1
          },
          {
            "id": "pole2",
            "weight": 1
          },
          {
            "id": "pole2",
            "weight": 1
          },
          {
            "id": "pole1",
            "weight": 1
          }
        ]
      }
    ],
    "dungeons": [
      {
        "id": "sub_steamchamber",
        "ambience": "alpha",
        "audio-ambience": "audio_4",
        "stretches": [
          {
            "tiles": [
              "steam_room"
            ]
          }
        ]
      },
      {
        "id": "sub_spidernest",
        "ambience": "delta",
        "audio-ambience": "audio_2",
        "stretches": [
          {
            "tiles": [
              "nest_1"
            ],
            "mobs": {
              "density": 3,
              "only": [
                "spidernest"
              ]
            }
          },
          {
            "tiles": [
              "nest_2"
            ],
            "mobs": {
              "density": 3,
              "only": [
                "spidernest"
              ]
            }
          },
          {
            "tiles": [
              "nest_3"
            ],
            "mobs": {
              "density": 2,
              "only": [
                "spidernest"
              ]
            }
          }
        ]
      },
      {
        "id": "sub_boobytrap",
        "ambience": "bravo",
        "audio-ambience": "audio_3",
        "stretches": [
          {
            "tiles": [
              "trap_1"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "trap_2"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "trap_3"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "trap_4"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "trap_5"
            ],
            "prop-groups": [
              "pole"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "trap_6"
            ],
            "prop-groups": [
              "pillar"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          }
        ]
      },
      {
        "id": "sub_troom",
        "ambience": "echo",
        "audio-ambience": "audio_6",
        "stretches": [
          {
            "tiles": [
              "troom_stretch"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "troom_middle"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "troom_middle_1"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "troom_end"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "arena-mix"
              ]
            }
          }
        ]
      },
      {
        "id": "sub_floodtemp",
        "ambience": "foxtrot",
        "audio-ambience": "audio_1",
        "stretches": [
          {
            "tiles": [
              "treasure_stairs"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "jungle-mix"
              ]
            }
          },
          {
            "tiles": [
              "treasure_path"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "jungle-mix"
              ]
            }
          },
          {
            "tiles": [
              "treasure_room"
            ],
            "mobs": {
              "density": 1,
              "only": [
                "jungle-mix"
              ]
            }
          }
        ]
      },
      {
        "id": "sub_templetunnel",
        "ambience": "bravo",
        "audio-ambience": "audio_5",
        "stretches": [
          {
            "tiles": [
              "tun_start"
            ],
            "mobs": {
              "density": 2,
              "only": [
                "arena-mix"
              ]
            }
          },
          {
            "tiles": [
              "tun_mid_5"
            ],
            "length": 1
          },
          {
            "tiles": [
              "tun_mid_6"
            ],
            "mobs": {
              "density": 2,
              "only": [
                "arena-mix"
              ]
            },
            "length": 1
          },
          {
            "tiles": [
              {
                "id": "tun_mid_1",
                "weight": 0.5
              },
              {
                "id": "tun_mid_2",
                "weight": 0.3
              },
              {
                "id": "tun_mid_joe",
                "weight": 0.2
              }
            ],
            "length": 1,
            "mobs": {
              "density": 2,
              "only": [
                "arena-mix"
              ]
            },
            "dead-ends": [
              {
                "id": "tun_mid_3",
                "weight": 0.7
              },
              {
                "id": "tun_dead_end",
                "weight": 0.3
              }
            ]
          },
          {
            "tiles": [
              "tun_right_2"
            ],
            "mobs": {
              "density": 2,
              "only": [
                "arena-mix"
              ]
            },
            "length": 1
          },
          {
            "tiles": [
              "tun_end"
            ],
            "length": 1
          }
        ]
      }
    ]
  }
