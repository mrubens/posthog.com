# PostHog Development Rules 🦔

Welcome to the PostHog development guidelines! Like a hedgehog navigating through a garden, we've got some prickly important rules to help you forage through code successfully.

## 🦔 The Hedgehog Philosophy

> "A hedgehog knows one big thing" - We focus on building the best product analytics platform, one spike at a time.

## 📝 Code Quality Rules

### Don't Be a Prick About Code Reviews

- **Be constructive, not destructive**: Like a hedgehog's quills, feedback should protect quality, not attack people
- **Review thoroughly**: Sniff out bugs like a hedgehog foraging for beetles
- **Respond promptly**: Don't hibernate on PRs - keep them moving!
- **Celebrate good code**: When you see something spike-tacular, say so!

### Spike Your Commits With Good Messages

Good commit messages are like hedgehog quills - sharp, pointed, and protective of code quality:

```bash
# Good (Spike-tacular!)
git commit -m "feat: add hedgehog animation to 404 page"
git commit -m "fix: prevent hedgehog from rolling off screen"
git commit -m "refactor: unroll nested hedgehog logic"

# Bad (Prickly situation!)
git commit -m "fixed stuff"
git commit -m "idk"
git commit -m "YOLO"
```

**Commit Message Format:**
- Use conventional commits: `feat:`, `fix:`, `docs:`, `refactor:`, etc.
- Keep the first line under 72 characters (a hedgehog is about 7 inches, so think compact!)
- Explain the "why" not just the "what"

### Curl Up Into a Ball When Debugging Gets Tough

When you encounter a gnarly bug:

1. **Don't panic-roll**: Take a breath, curl up, and assess the situation
2. **Isolate the problem**: Like finding the right quill in a bundle, narrow down the issue
3. **Use the debugger**: Don't just console.log your way through life (though hedgehogs do leave trails...)
4. **Ask for help**: Even hedgehogs travel in groups sometimes (they're called "arrays" of hedgehogs!)
5. **Document the solution**: Help future hedgehogs avoid the same prickly situation

### Forage Before You Ask

Before asking questions, do some hedgehog-style foraging:

- 🔍 Search the docs at [`posthog.com/docs`](https://posthog.com/docs)
- 🔍 Check existing issues on GitHub
- 🔍 Look through the codebase for similar implementations
- 🔍 Try the PostHog community at [`posthog.com/questions`](https://posthog.com/questions)

If you still need help after foraging, that's totally fine! We're a friendly array of hedgehogs here.

## 🏗️ Architecture & Design

### Keep It Simple, Hedgehog

- **KISS Principle**: Keep It Simple, Spiky
- **Avoid over-engineering**: A hedgehog doesn't need rocket boosters to cross the garden
- **Prefer composition over inheritance**: Like quills on a hedgehog, build from small, reusable pieces
- **Write code for hedgehogs, not computers**: Make it readable for the next developer

### Don't Reinvent the Wheel (or the Hedgehog)

- Check if a solution already exists before building from scratch
- Use established patterns and libraries
- When in doubt, ask: "Would a hedgehog do it this way?"

## 🧪 Testing Rules

### Test Like Your Code Will Hibernate

Write tests that will still work when you wake up from hibernation:

- **Unit tests**: Test individual quills, not the whole hedgehog
- **Integration tests**: Make sure the quills work together
- **E2E tests**: Ensure the hedgehog can actually cross the garden
- **Coverage**: Aim for good coverage, but don't be prickly about 100%

```typescript
// Good test naming - clear as a hedgehog's path
describe('HedgehogAnimation', () => {
  it('should roll into a ball when scared', () => {
    // Test implementation
  })
  
  it('should unroll when safe', () => {
    // Test implementation
  })
})

// Bad test naming - as confusing as a lost hedgehog
describe('HA', () => {
  it('works', () => {
    // What works? Nobody knows!
  })
})
```

## 📚 Documentation

### Document Like You're Teaching a Baby Hedgehog

- **Be clear and concise**: Baby hedgehogs (hoglets!) need simple explanations
- **Include examples**: Show, don't just tell
- **Keep it updated**: Outdated docs are like old quills - they need replacing
- **Use hedgehog humor**: Make it fun! (You're reading this, aren't you?)

### README Files Should Be Spike-tacular

Every significant directory should have a README that answers:
- What does this code do?
- Why does it exist?
- How do I use it?
- Where can I learn more?

## 🚀 Deployment & Release

### Roll Carefully Into Production

- **Test thoroughly**: Don't roll into production with your quills down
- **Use feature flags**: Roll out features gradually, like a cautious hedgehog
- **Monitor closely**: Watch for issues like a hedgehog watches for predators
- **Have a rollback plan**: Sometimes you need to curl back up quickly

### Semantic Versioning: The Hedgehog Way

- **MAJOR**: Breaking changes (hedgehog learned to fly - whoa!)
- **MINOR**: New features (hedgehog learned a new foraging spot)
- **PATCH**: Bug fixes (hedgehog fixed a bent quill)

## 🤝 Collaboration

### Be a Team Hedgehog, Not a Lone Quill

- **Communicate early and often**: Hedgehogs grunt to each other for a reason
- **Share knowledge**: Don't hoard information like a hedgehog hoards beetles
- **Pair program**: Two hedgehogs are better than one
- **Celebrate wins**: Do a little hedgehog victory roll!

### Code Ownership: We're All in This Burrow Together

- No code is "owned" by one person
- Everyone can contribute to any part of the codebase
- Leave code better than you found it (the hedgehog scout rule)
- Don't be territorial - we're not badgers!

## 🔒 Security

### Protect Like a Hedgehog Protects Its Belly

- **Never commit secrets**: Keep your soft underbelly protected
- **Validate all inputs**: Don't trust anything that rolls into your burrow
- **Use environment variables**: Keep secrets in `.env` files (and `.gitignore` them!)
- **Review security patches**: Stay sharp like fresh quills

### Authentication & Authorization

- Always authenticate users before they can access the burrow
- Use proper authorization checks - not every hedgehog should access every quill
- Follow the principle of least privilege - only give access to what's needed

## 🎨 Code Style

### Keep Your Quills Aligned

We use automated formatters, so you don't have to worry about alignment:

- **Prettier**: For JavaScript/TypeScript (auto-formats on save)
- **ESLint**: For catching bugs and enforcing patterns
- **TypeScript**: For type safety (hedgehogs hate runtime surprises!)

### Naming Conventions: Clear as a Hedgehog's Trail

```typescript
// Components: PascalCase
const HedgehogAnimation = () => { }

// Functions: camelCase
function rollIntoABall() { }

// Constants: SCREAMING_SNAKE_CASE
const MAX_HEDGEHOG_SPEED = 6 // mph

// Private variables: _leadingUnderscore (but prefer TypeScript private)
class Hedgehog {
  private _quillCount = 5000
}
```

## 🐛 Bug Reporting

### When You Find a Bug: Don't Just Roll Away!

Create a detailed bug report with:

1. **Title**: Clear and descriptive (e.g., "Hedgehog animation stutters on mobile")
2. **Description**: What happened vs. what should happen
3. **Steps to reproduce**: Help others find the same prickly issue
4. **Environment**: Browser, OS, device (where was the hedgehog when it happened?)
5. **Screenshots/Videos**: A picture is worth a thousand quills

## 🌟 Performance

### Fast as a Hedgehog (When It Needs to Be)

Hedgehogs aren't the fastest animals, but they know when to hurry:

- **Optimize when needed**: Don't prematurely optimize (hedgehogs don't sprint everywhere)
- **Measure first**: Use profiling tools before optimizing
- **Lazy load**: Like a hedgehog saving energy, only load what's needed
- **Cache wisely**: Store frequently used data (like a hedgehog's favorite foraging spots)

### Bundle Size: Keep It Hedgehog-Sized

- Monitor bundle sizes - we're building a website, not a elephant
- Code split when appropriate
- Use dynamic imports for heavy features
- Tree-shake unused code (shake off those dead quills!)

## 🎯 Accessibility

### Make It Accessible for All Hedgehogs

- **Semantic HTML**: Use proper elements (hedgehogs need structure!)
- **ARIA labels**: Help screen readers navigate the burrow
- **Keyboard navigation**: Not all hedgehogs use mice (pun intended!)
- **Color contrast**: Make sure hedgehogs with poor eyesight can see too
- **Alt text**: Describe images for hedgehogs who can't see them

## 🌍 Internationalization

### Think Global, Act Hedgehog

- Use i18n for all user-facing strings
- Don't hardcode text (hedgehogs speak many languages!)
- Consider RTL languages (some hedgehogs read right-to-left)
- Be culturally sensitive (not all cultures appreciate hedgehog puns... okay, most do)

## 📱 Responsive Design

### Roll Smoothly Across All Devices

- **Mobile first**: Start small, like a baby hedgehog (hoglet!)
- **Test on real devices**: Emulators are nice, but real hedgehogs matter
- **Touch targets**: Make buttons big enough for hedgehog paws (44x44px minimum)
- **Performance on mobile**: Mobile hedgehogs have less processing power

## 🔄 Git Workflow

### Branch Like a Hedgehog's Burrow System

```bash
# Main branches
main          # Production - the main burrow
develop       # Development - the construction site

# Feature branches
feature/hedgehog-animation
feature/spike-counter
fix/rolling-bug
hotfix/critical-quill-issue
```

### Pull Request Checklist: The Hedgehog Pre-Roll Inspection

Before requesting a PR review:

- [ ] Code builds without errors (no broken quills)
- [ ] Tests pass (hedgehog can roll properly)
- [ ] Linting passes (quills are aligned)
- [ ] Documentation updated (other hedgehogs know what you did)
- [ ] Screenshots added (if UI changes - show off that hedgehog!)
- [ ] Self-reviewed (you checked your own quills first)
- [ ] Branch is up to date with main (no merge conflicts - hedgehogs don't fight)

## 🎓 Learning Resources

### Become a Wise Hedgehog

- 📖 [PostHog Docs](https://posthog.com/docs) - The hedgehog handbook
- 💬 [PostHog Questions](https://posthog.com/questions) - Ask the array
- 🐙 [GitHub Repo](https://github.com/PostHog/posthog) - The main burrow
- 📰 [PostHog Blog](https://posthog.com/blog) - Hedgehog wisdom
- 🎥 [PostHog YouTube](https://www.youtube.com/@PostHog) - Video tutorials for visual hedgehogs

## 🎉 Fun Rules

### Keep the Hedgehog Spirit Alive

- **Hedgehog Friday**: Share hedgehog memes in Slack
- **Name your test data**: Use hedgehog-themed names (Max, Spike, Quilly, etc.)
- **Celebrate launches**: Do a hedgehog roll when features ship!
- **Hedgehog of the month**: Recognize outstanding contributions
- **Easter eggs**: Hide hedgehog references in the code (you found one by reading this!)

## 🚨 When Things Go Wrong

### Emergency Hedgehog Procedures

If production is on fire (metaphorically - hedgehogs don't like fire):

1. **Stay calm**: Panicked hedgehogs make poor decisions
2. **Communicate**: Alert the team immediately
3. **Assess**: What's broken? How bad is it?
4. **Mitigate**: Can we roll back? Feature flag it off?
5. **Fix**: Address the root cause
6. **Post-mortem**: Learn from it (no blame, just growth)

### The Hedgehog Hotfix Process

```bash
# Create hotfix branch from main
git checkout main
git checkout -b hotfix/critical-spike-issue

# Fix the issue (quickly but carefully!)
# Test thoroughly (even in emergencies, test!)
# Create PR with "HOTFIX" label
# Get expedited review
# Merge and deploy
# Backport to develop

# Breathe - the hedgehog lives another day!
```

## 🦔 The Golden Hedgehog Rules

Remember these above all else:

1. **Be kind**: We're all hedgehogs trying our best
2. **Be curious**: Ask questions, explore, learn
3. **Be thorough**: Test your code, review carefully
4. **Be communicative**: Share early, share often
5. **Be proud**: You're building something spike-tacular!
6. **Have fun**: If you're not enjoying it, you're doing it wrong

---

## 🎯 Final Words of Hedgehog Wisdom

> "The hedgehog knows many things, but the fox knows one big thing." - We know product analytics, and we're damn good at it.

Remember: Every line of code you write is a quill in PostHog's armor. Make it count. Make it good. Make it hedgehog-worthy.

Now go forth and code, you magnificent hedgehog! 🦔✨

---

*Last updated: When hedgehogs learned to code*  
*Maintained by: The entire array of PostHog hedgehogs*  
*Questions? Visit [posthog.com/questions](https://posthog.com/questions)*

**P.S.** If you read this entire document, you deserve a virtual hedgehog high-five! 🦔✋