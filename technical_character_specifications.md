# Technical Character Specifications

## Core Philosophy

**"Cultural detail through technical precision"** - Technical specifications must support authentic Thai cultural representation while maintaining smooth gameplay performance and modern visual standards.

## Sprite Dimension Standards

### Character Size Hierarchy
**Protagonist Evolution Sizing**: Spiritual development reflected through sprite size progression

#### Broken State Specifications
**Base Dimensions**: 48x64 pixels
- **Rationale**: Smaller size reflecting diminished spiritual presence and collapsed posture
- **Detail Allocation**: Sufficient space for basic emotional states, minimal cultural detail
- **Performance**: Lightweight for opening sequence and memory-constrained situations
- **Animation Capability**: 4-6 frames maximum for basic movement and breathing

**Cultural Detail Limitations**:
- **Face Area**: 8x10 pixels - basic expressions only
- **Clothing Detail**: 16x20 pixels - modern street clothes, no traditional elements
- **Weapon Integration**: 12x24 pixels - krabong appears crude, basic wooden staff
- **Amulet Display**: None - complete spiritual disconnection

#### Awakening State Specifications  
**Base Dimensions**: 52x68 pixels
- **Rationale**: Growing confidence and spiritual awareness reflected in improved posture
- **Detail Enhancement**: Increased space for cultural learning and emotional development
- **Performance**: Balanced between detail and efficiency for mid-game content
- **Animation Capability**: 6-8 frames for developing martial arts and cultural interactions

**Cultural Detail Development**:
- **Face Area**: 10x12 pixels - basic Thai emotional vocabulary possible
- **Clothing Detail**: 18x24 pixels - simple traditional elements beginning to appear
- **Weapon Integration**: 14x28 pixels - krabong showing better proportion, faint patterns
- **Amulet Display**: 8x10 pixels - single basic amulet display capability

#### Warrior State Specifications
**Base Dimensions**: 56x72 pixels  
- **Rationale**: Full spiritual presence and cultural integration, maximum detail capability
- **Detail Mastery**: Complete space for authentic Thai cultural representation
- **Performance**: Optimized high-detail sprite for endgame content and key sequences
- **Animation Capability**: 12-16 frames for complex techniques and cultural interactions

**Cultural Detail Mastery**:
- **Face Area**: 12x16 pixels - full Thai emotional vocabulary and micro-expressions
- **Clothing Detail**: 20x30 pixels - complete sarong system with authentic tribal patterns
- **Weapon Integration**: 16x32 pixels - krabong with full sacred geometry and yantra patterns
- **Amulet Display**: 16x12 pixels - multiple amulets with individual detail and glow effects

### Enemy Sprite Hierarchy
**Spiritual Corruption Reflected in Size and Detail**: Visual hierarchy showing moral/spiritual status

#### Street Level Antagonists
**Thug Specifications**: 44x64 pixels
- **Rationale**: Smaller than protagonist showing diminished spiritual presence
- **Detail Focus**: Crude modern clothing, artificial materials, spiritual emptiness
- **Animation**: 4-6 frames, basic aggressive movements, no spiritual techniques
- **Cultural Elements**: Complete absence of authentic Thai cultural items

**Gang Leader Specifications**: 46x66 pixels
- **Rationale**: Slightly larger than thugs but smaller than spiritually developed protagonist
- **Detail Focus**: Expensive but tasteless clothing, corrupted traditional symbols
- **Animation**: 6-8 frames, basic authority gestures, false confidence movements
- **Cultural Elements**: Misused Thai symbols, fake spiritual objects

#### Institutional Corruption
**Corrupt Official Specifications**: 50x68 pixels
- **Rationale**: Professional appearance requiring detail, but spiritually empty
- **Detail Focus**: Expensive suits, corrupted authority symbols, false respectability
- **Animation**: 8-10 frames, professional movements hiding criminal nature
- **Cultural Elements**: Traditional authority symbols used inappropriately

**False Monk Specifications**: 52x70 pixels
- **Rationale**: Sacred robes require detail accuracy, spiritual corruption shown subtly
- **Detail Focus**: Proper saffron robes with hidden corruption indicators
- **Animation**: 10-12 frames, proper monastic movements hiding criminal activity
- **Cultural Elements**: Authentic appearance with subtle corruption markers

#### Spiritual Entities
**Malevolent Spirit Specifications**: 48x72 pixels
- **Rationale**: Supernatural height showing otherworldly power
- **Detail Focus**: Traditional Thai supernatural aesthetics with urban corruption
- **Animation**: 8-12 frames, floating/supernatural movement patterns
- **Cultural Elements**: Authentic traditional ghost forms corrupted by modern evil

**Guardian Spirit Specifications**: 56x80 pixels
- **Rationale**: Largest enemies showing supernatural guardian power
- **Detail Focus**: Traditional yaksha appearance with corruption or purity indicators
- **Animation**: 12-16 frames, powerful guardian movements and spiritual effects
- **Cultural Elements**: Authentic Thai guardian aesthetics with moral alignment visualization

## Modular Component Architecture

### Protagonist Component System
**Efficient Cultural Customization**: Supporting authentic combinations without memory bloat

#### Base Character Components
**Core Sprite Elements**:
- **Body Base**: 32x48 pixels - unchanging body structure across all customization
- **Head/Face**: 12x16 pixels - separate component for expression changes
- **Arms**: 8x24 pixels each - separate for different poses and weapon handling
- **Legs**: 12x32 pixels - separate for different stances and movement styles

**Technical Integration**:
- **Assembly System**: Components combined in real-time based on current state
- **Memory Efficiency**: Shared components across similar configurations
- **Animation Synchronization**: Component animation synchronized for natural movement
- **Performance Scaling**: Component detail adjustable based on hardware capability

#### Cultural Customization Layers
**Sarong System Components**:
- **Base Sarong**: 20x30 pixels - foundation sarong shape and color
- **Pattern Overlay**: 16x24 pixels - authentic tribal pattern details
- **Length Variation**: 3 different length components (long, medium, short)
- **Regional Styles**: Northern, Central, Southern component variations

**Technical Implementation**:
- **Pattern Library**: 16x24 pixel authentic pattern tiles for cultural accuracy
- **Color Palette**: Regional color schemes maintaining cultural authenticity
- **Physics Integration**: Length affects animation and movement physics
- **Cultural Verification**: Pattern combinations checked against cultural appropriateness

#### Amulet Display System
**Multiple Amulet Management**:
- **Primary Amulet**: 8x12 pixels - most prominent amulet display
- **Secondary Amulets**: 6x8 pixels each - additional amulets without crowding
- **Glow Effects**: 2-pixel radius spiritual energy around authentic amulets
- **Combination Effects**: Visual harmony when amulets work together

**Performance Optimization**:
- **Active Limit**: Maximum 3 visible amulets to prevent visual crowding
- **LOD System**: Amulet detail reduces with camera distance
- **Effect Culling**: Spiritual effects removed when off-camera
- **Cultural Database**: Efficient lookup for amulet authenticity and compatibility

### Animation Frame Management

#### Movement Animation Economics
**Standard Action Frame Counts**:

**Basic Movement**:
- **Idle**: 6 frames, 0.4s each - subtle breathing and alertness
- **Walk**: 8 frames, 0.1s each - natural gait with sarong physics
- **Run**: 8 frames, 0.08s each - urgent movement with fabric dynamics
- **Cultural Walk**: 10 frames, 0.12s each - respectful temple/formal pace

**Combat Actions**:
- **Basic Attacks**: 8-10 frames, 0.06s each - readable technique with cultural accuracy
- **Special Moves**: 16-20 frames, variable timing - signature techniques with spiritual effects
- **Defensive Actions**: 6-8 frames, 0.04s each - reactive blocking and dodging
- **Finishers**: 24+ frames, 0.08s each - dramatic cultural showcase with karma implications

#### Cultural Interaction Animations
**Thai Social Behavior**:
- **Wai Greeting**: 6 frames, 0.3s each - proper Thai greeting with regional variations
- **Temple Prostration**: 12 frames, 0.25s each - respectful Buddhist prostration sequence
- **Amulet Blessing**: 8 frames, 0.2s each - touching amulets for spiritual activation
- **Meditation Transition**: 10 frames, 0.3s each - entering and exiting meditation states

**Technical Requirements**:
- **Cultural Accuracy**: All social animations verified by Thai cultural consultants
- **Regional Variations**: Different animation variations for Northern, Central, Southern styles
- **Context Sensitivity**: Animations automatically selected based on social context
- **Respect Integration**: Proper cultural behavior unlocks positive NPC interactions

## Memory and Performance Optimization

### Sprite Sheet Organization
**Efficient Resource Management**: Maximizing cultural detail while minimizing memory usage

#### Character State Organization
**Protagonist Sprite Sheets**:
- **Broken State Sheet**: 512x512 pixels - complete broken state animations and expressions
- **Awakening State Sheet**: 1024x512 pixels - expanded animation set with cultural development
- **Warrior State Sheet**: 1024x1024 pixels - full animation set with complete cultural integration
- **Modular Components**: Separate sheets for sarongs, amulets, weapons, cultural accessories

**Loading Strategy**:
- **Progressive Loading**: Higher detail states loaded as character develops
- **Component Caching**: Frequently used components kept in memory
- **Cultural Asset Streaming**: Regional components loaded based on current location
- **Performance Scaling**: Asset quality adjusted based on hardware capability

#### Enemy Sprite Optimization
**Corruption Hierarchy Management**:
- **Shared Corruption Elements**: Common visual corruption indicators across enemy types
- **Modular Enemy Design**: Base enemy forms with corruption/purity overlay systems
- **Cultural Element Library**: Shared authentic vs. corrupted cultural symbol library
- **Performance Grouping**: Similar enemies share sprite components and animation cycles

### Real-Time Cultural Verification
**Authentic Combination Validation**: Ensuring cultural authenticity without performance impact

#### Cultural Database Integration
**Authenticity Checking**:
- **Pattern Compatibility**: Real-time verification of sarong pattern combinations
- **Regional Appropriateness**: Location-based cultural element validation  
- **Historical Accuracy**: Time period verification for historical element combinations
- **Spiritual Consistency**: Buddhist principle verification for amulet combinations

**Technical Implementation**:
- **Hash-Based Lookup**: Fast authenticity verification using pre-computed hashes
- **Cultural Rules Engine**: Efficient rule evaluation for complex cultural interactions
- **Performance Caching**: Cultural verification results cached to prevent repeated calculations
- **Graceful Degradation**: Cultural verification scales based on available processing power

### Hardware Scaling and Accessibility

#### Performance Adaptation
**Multi-Tier Quality System**:

**High Performance Mode**:
- **Full Resolution**: All sprites at maximum specified dimensions
- **Complete Animation**: All animation frames with full timing precision
- **Cultural Detail**: Maximum authentic pattern detail and spiritual effects
- **Real-Time Verification**: Full cultural authenticity checking

**Standard Performance Mode**:
- **Optimized Resolution**: 90% of maximum sprite dimensions
- **Reduced Animation**: Key frames with interpolation for smooth movement
- **Simplified Detail**: Core cultural elements maintained, complex patterns simplified
- **Periodic Verification**: Cultural authenticity checked less frequently

**Low Performance Mode**:
- **Compact Resolution**: 75% of maximum dimensions for memory efficiency
- **Essential Animation**: Core movement and combat frames only
- **Basic Detail**: Fundamental cultural elements, minimal decorative detail
- **Cached Verification**: Cultural rules pre-calculated and cached

#### Accessibility Features
**Visual Accessibility**:
- **High Contrast Mode**: Enhanced contrast for cultural pattern visibility
- **Color Blind Support**: Alternative color schemes maintaining cultural meaning
- **Text Scaling**: Larger text overlays for cultural information and tutorials
- **Pattern Recognition Aids**: Enhanced highlighting for authentic vs. corrupted elements

**Cultural Accessibility**:
- **Cultural Tutorial Mode**: Enhanced explanations for non-Thai players
- **Pronunciation Guides**: Audio pronunciation for Thai cultural terms
- **Cultural Context**: Optional cultural background information overlays
- **Respectful Learning**: Gradual introduction to complex cultural concepts

---

**Navigation**: [← Character Animation Language](./character-animation-language.md) | [Character Design](../character-design.md)

**Related**: [Art Direction](../art-direction.md) | [Cultural Elements](../../cultural-elements.md) | [Technical Specifications](../technical-specifications.md)