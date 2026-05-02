# 🎮 RokueQuest - A Roguelike Adventure with Java

A thrilling roguelike adventure game built entirely in Java, featuring procedurally generated dungeons, turn-based combat, character progression, and challenging enemy encounters.

## 🎯 Overview

RokueQuest is a classic roguelike dungeon crawler that brings the excitement of retro gaming to modern platforms. Navigate through procedurally generated dungeons, battle fearsome monsters, collect loot, and uncover secrets in a world full of danger and adventure. With strategic turn-based combat and permadeath mechanics, every playthrough is a unique challenge.

## ✨ Features

### 🗺️ Procedurally Generated Dungeons
- **Dynamic Level Generation** - Each dungeon is uniquely generated every playthrough
- **Multiple Dungeon Levels** - Progressively challenging environments
- **Environmental Hazards** - Traps, environmental obstacles, and dangerous terrain
- **Hidden Treasures** - Secret rooms and hidden loot waiting to be discovered
- **Random Encounters** - Unpredictable enemy placement and encounters

### ⚔️ Combat System
- **Turn-Based Combat** - Strategic tactical gameplay
- **Multiple Attack Types** - Melee, ranged, and special abilities
- **Enemy AI** - Intelligent enemies with different behaviors and strategies
- **Boss Encounters** - Challenging unique boss battles at level ends
- **Status Effects** - Poison, stun, bleed, and other status conditions
- **Combat Log** - Detailed tracking of all battle events

### 👤 Character System
- **Character Classes** - Warrior, Rogue, Mage, and Ranger with unique abilities
- **Experience and Leveling** - Grow stronger as you progress
- **Skill Trees** - Develop your character with specialized abilities
- **Equipment System** - Find, equip, and manage weapons and armor
- **Stat Progression** - Strength, Dexterity, Intelligence, and Endurance

### 🎁 Loot and Rewards
- **Random Loot Drops** - Defeat enemies to find valuable items
- **Equipment Rarity Tiers** - Common, Uncommon, Rare, Epic, and Legendary items
- **Potion and Consumables** - Health potions, mana potions, and special consumables
- **Gold Currency** - Collect gold for shopping and upgrades
- **Crafting System** - Combine items to create new equipment and potions

### 🏆 Progression and Scoring
- **Permadeath Mechanic** - Classic roguelike permanent death system
- **Highscore Leaderboard** - Track your best runs and compete with friends
- **Achievement System** - Unlock achievements for special accomplishments
- **Stats Tracking** - Monitor kills, damage dealt, floors cleared, and more
- **Difficulty Scaling** - Increasing challenge as you progress deeper

### 🎨 User Interface
- **Intuitive Controls** - Easy to learn, challenging to master
- **Real-time Statistics** - Monitor health, mana, equipment, and inventory
- **Inventory Management** - Organize and manage your items
- **Detailed Info Panels** - Learn about enemies, items, and abilities
- **Turn History** - Review previous actions and decisions

## 🛠️ Tech Stack

- **Language:** Java
- **Architecture:** Object-Oriented Design
- **UI Framework:** Swing (Desktop) or JavaFX (Modern UI)
- **Game Engine:** Custom built-in engine
- **Data Persistence:** Serialization for saving game state

## 📋 Requirements

- Java 8 or higher
- JVM (Java Virtual Machine)
- 100MB disk space
- Windows, macOS, or Linux

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/cago8/RokueQuest-A-Roguelike-Adventure-with-Java.git
cd RokueQuest-A-Roguelike-Adventure-with-Java
```

### Build the Project

```bash
# Using Maven
mvn clean package

# Or using Gradle
gradle build

# Or compile manually
javac -d bin src/**/*.java
```

### Run the Game

```bash
# Using Maven
mvn exec:java -Dexec.mainClass="com.rokuequest.Main"

# Or using Gradle
gradle run

# Or run the JAR
java -jar target/RokueQuest.jar

# Or run compiled classes
java -cp bin com.rokuequest.Main
```

## 🚀 Getting Started

### 1. Start a New Game

1. Launch the application
2. Click **"New Game"**
3. Select your character class:
   - **Warrior:** High HP, strong melee attacks
   - **Rogue:** High speed, critical strikes, evasion
   - **Mage:** Powerful spells, mana-based abilities
   - **Ranger:** Long-range attacks, status effects

### 2. Navigate the Dungeon

- **Arrow Keys** or **WASD** - Move around
- **Space** - Interact with objects
- **I** - Open inventory
- **C** - Character stats
- **Q** - Quest log

### 3. Combat

- **Attack enemies** - Automatically target adjacent enemies
- **Use abilities** - Press number keys (1-9) to use abilities
- **Use items** - Select items from inventory during combat
- **Run away** - Attempt to escape dangerous encounters

### 4. Progression

- **Defeat enemies** - Gain experience and loot
- **Level up** - Choose stat improvements or new abilities
- **Find better equipment** - Equip stronger weapons and armor
- **Descend deeper** - Progress to harder dungeon levels
- **Defeat the boss** - Complete each level's final challenge

## 📁 Project Structure

```
RokueQuest-A-Roguelike-Adventure-with-Java/
├── src/
│   ├── com/rokuequest/
│   │   ├── Main.java              # Entry point
│   │   ├── Game.java              # Core game loop
│   │   ├── entities/
│   │   │   ├── Player.java
│   │   │   ├── Enemy.java
│   │   │   └── Boss.java
│   │   ├── items/
│   │   │   ├── Item.java
│   │   │   ├── Weapon.java
│   │   │   ├── Armor.java
│   │   │   └── Potion.java
│   │   ├── dungeon/
│   │   │   ├── Dungeon.java
│   │   │   ├── Room.java
│   │   │   ├── DungeonGenerator.java
│   │   │   └── Tile.java
│   │   ├── abilities/
│   │   │   ├── Ability.java
│   │   │   ├── AttackAbility.java
│   │   │   └── SpellAbility.java
│   │   ├── ui/
│   │   │   ├── GameWindow.java
│   │   │   ├── GamePanel.java
│   │   │   └── UIManager.java
│   │   └── utils/
│   │       ├── Random.java
│   │       ├── FileManager.java
│   │       └── Constants.java
├── resources/
│   ├── sprites/               # Game graphics
│   ├── sounds/                # Sound effects
│   └── config/                # Game configuration files
├── pom.xml                    # Maven configuration
├── build.gradle               # Gradle configuration
└── README.md
```

## 🎮 Game Mechanics

### Character Classes

#### Warrior
```
HP: 100  | Strength: 18  | Dexterity: 10  | Intelligence: 8
- High health pool
- Strong melee attacks
- Armor proficiency bonus
- Special: Whirlwind Attack
```

#### Rogue
```
HP: 70   | Strength: 14  | Dexterity: 18  | Intelligence: 10
- High evasion chance
- Critical strike bonus
- Stealth abilities
- Special: Shadow Clone
```

#### Mage
```
HP: 60   | Strength: 8   | Dexterity: 12  | Intelligence: 18
- Large mana pool
- Powerful spells
- Area of effect abilities
- Special: Meteor Storm
```

#### Ranger
```
HP: 80   | Strength: 12  | Dexterity: 16  | Intelligence: 12
- Long-range attacks
- Status effect arrows
- Trap abilities
- Special: Arrow Barrage
```

### Combat System

**Turn Order:** Speed-based (Dexterity stat)

**Attack Roll:**
```
Hit Chance = Base Accuracy + (Dexterity / 10) - Enemy Defense
Critical Chance = (Dexterity % 10) + 5
```

**Damage Calculation:**
```
Damage = Base Weapon Damage + (Strength / 5) + Enchantments
Final Damage = Damage * Critical Multiplier - Enemy Armor
```

### Loot Rarities

| Rarity | Color | Drop Rate | Stats |
|--------|-------|-----------|-------|
| Common | Gray | 60% | +1-2 Stats |
| Uncommon | Green | 25% | +3-5 Stats |
| Rare | Blue | 10% | +6-10 Stats |
| Epic | Purple | 4% | +11-20 Stats |
| Legendary | Gold | 1% | +21-50 Stats |

### Dungeon Levels

| Level | Difficulty | Enemies | Boss | Reward |
|-------|-----------|---------|------|--------|
| 1 | Easy | Goblins, Wolves | Goblin King | Iron Sword |
| 2 | Normal | Orcs, Spiders | Spider Queen | Steel Armor |
| 3 | Hard | Demons, Wraiths | Shadow Lord | Gold Sword |
| 4 | Very Hard | Liches, Dragons | Ancient Dragon | Legendary Weapon |

## 🎯 Abilities and Spells

### Warrior Abilities
- **Power Attack** - Deal 150% damage (cooldown: 1 turn)
- **Shield Bash** - Stun enemy and reduce damage (cooldown: 2 turns)
- **Whirlwind** - Attack all enemies around (cooldown: 3 turns)

### Rogue Abilities
- **Backstab** - Deal 200% damage from behind (cooldown: 1 turn)
- **Evasion** - Dodge next attack (cooldown: 2 turns)
- **Shadow Clone** - Create duplicate to attack (cooldown: 4 turns)

### Mage Spells
- **Fireball** - AOE fire damage (Mana cost: 15)
- **Freeze** - Stun enemies in radius (Mana cost: 20)
- **Meteor Storm** - Massive AOE damage (Mana cost: 50)

### Ranger Abilities
- **Multishot** - Fire multiple arrows (cooldown: 1 turn)
- **Poison Arrow** - Apply poison status (cooldown: 2 turns)
- **Explosive Trap** - Place damaging trap (cooldown: 2 turns)

## 🧪 Testing

Run the test suite:

```bash
# Using Maven
mvn test

# Using Gradle
gradle test

# Or run directly
java -cp bin:test org.junit.runner.JUnitCore TestSuite
```

## 📊 Sample Run

```
=== RokueQuest ===
[1] New Game
[2] Continue
[3] Highscores
[4] Exit

Choose: 1

Select Character:
[1] Warrior
[2] Rogue
[3] Mage
[4] Ranger

Choose: 2

=== Level 1: Goblin Caves ===
You have entered the dungeon!

Rogue HP: 70/70 | XP: 0/100

[X . . E . ]
[. . . . . ]
[. . @ . . ]
[. . . . . ]
[. . . . . ]

[1] Move
[2] Attack
[3] Use Ability
[4] Use Item
[5] Stats

Action: 1
Direction: Up
Moved to position (2, 2)

A Goblin appears!
Combat Started!

Rogue uses Backstab
Hit! 45 damage to Goblin
Goblin is defeated!
Loot: Iron Dagger, 50 Gold

Continue...
```

## 🐛 Bug Reports

Found a bug? Report it:

1. Go to [Issues](https://github.com/cago8/RokueQuest-A-Roguelike-Adventure-with-Java/issues)
2. Click **"New Issue"**
3. Describe the problem and how to reproduce it
4. Include screenshots if applicable

## 📧 Contact & Support

For questions or support:

- **Email:** [cagribilginer60@gmail.com](mailto:cagribilginer60@gmail.com)
- **GitHub Issues:** [Report Issues](https://github.com/cago8/RokueQuest-A-Roguelike-Adventure-with-Java/issues)
- **GitHub Discussions:** [Start Discussion](https://github.com/cago8/RokueQuest-A-Roguelike-Adventure-with-Java/discussions)

## 🤝 Contributing

We welcome contributions! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add: YourFeature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

### Contribution Ideas
- New character classes
- Additional abilities and spells
- More enemy types
- Improved dungeon generation
- UI/UX improvements
- Sound and music
- Performance optimization

## 📜 License

This project is open source and available under the **MIT License**.

See the [LICENSE](LICENSE) file for details.

## 🎓 Learning Resources

This project is excellent for learning:

- **Object-Oriented Programming** - Class hierarchies and design patterns
- **Game Development** - Game loops, entity management, collision detection
- **Data Structures** - Grids, trees, and pathfinding algorithms
- **AI Programming** - Enemy behavior and decision making
- **File I/O** - Save/load game state
- **UI Development** - Building interactive user interfaces with Swing/JavaFX
- **Procedural Generation** - Creating random but coherent game content

## 🙏 Acknowledgments

- Inspired by classic roguelikes like Rogue, Nethack, and Dungeon Crawl
- Built with Java for cross-platform compatibility
- Thanks to the Java gaming community

## 📈 Roadmap

Planned features:

- [ ] Multiplayer support
- [ ] More character classes (Paladin, Necromancer, etc.)
- [ ] Expanded skill trees
- [ ] New enemy types and bosses
- [ ] Improved graphics and animations
- [ ] Sound effects and music
- [ ] Mobile version
- [ ] Online leaderboards
- [ ] Daily challenges
- [ ] Mod support

## 🔗 Quick Links

- **Repository:** https://github.com/cago8/RokueQuest-A-Roguelike-Adventure-with-Java
- **Issues:** https://github.com/cago8/RokueQuest-A-Roguelike-Adventure-with-Java/issues
- **Wiki:** [Game Guide and Documentation]

---

**Made with ❤️ by Çağrı BİLGİNER**

*Venture forth, brave adventurer! Death awaits in the dungeons below! ⚔️🐉*
