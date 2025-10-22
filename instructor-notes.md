# Cybersecurity Acronyms Jeopardy - Instructor Notes

## Overview
This is a Jeopardy-style educational game designed to teach cybersecurity acronyms in an engaging, competitive format. The game progresses from basic to advanced topics with increasing point values corresponding to difficulty.

## Game Setup

### Technical Requirements
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No internet connection required (standalone HTML file)
- Works on desktop, tablet, and mobile devices
- Projector or large screen recommended for classroom use

### Pre-Game Setup
1. Open `cybersecurity-jeopardy.html` in a web browser
2. Test the flip card functionality before class
3. Decide on team composition (suggested: 3 teams of 3-5 players)
4. Have a way to track which team answers (raise hands, buzzers, etc.)

## Game Rules & Flow

### Standard Play
1. **Team Selection**: Teams take turns selecting a category and point value
2. **Question Display**: Click the selected card to display the question
3. **Answer Period**: Teams have 30 seconds to discuss and answer
4. **Reveal Answer**: Click "Reveal Answer" to flip the card and show the correct answer
5. **Scoring**:
   - Award points for correct answers using the +100/+200/+300 buttons
   - Deduct points for incorrect answers using the -100 button (optional)
6. **Card Marking**: Used cards automatically gray out
7. **Next Turn**: Close modal and allow next team to select

### Alternate Play Modes

#### Buzzer Mode
- Display question to all teams simultaneously
- First team to buzz in gets to answer
- If incorrect, other teams can steal

#### Daily Double (Advanced)
- Instructor secretly designates 2-3 cards as "Daily Doubles"
- Team can wager up to their current score
- Only that team gets to answer

## Category Breakdown

### 1. Basic Security (Easiest)
**Target Audience**: Beginners, general awareness training

- **$100 - VPN**: Most common term, widely used in corporate environments
- **$200 - SSL**: Foundation of web security
- **$300 - MFA**: Current best practice for authentication
- **$400 - AES**: Standard encryption algorithm
- **$500 - PKI**: Infrastructure concept, slightly more complex

**Teaching Tips**:
- Emphasize practical applications (VPN for remote work, SSL for websites)
- Relate MFA to everyday experiences (phone + password)

### 2. Threats & Attacks
**Target Audience**: Security awareness, SOC analysts, defenders

- **$100 - DoS**: Simple concept of overwhelming a system
- **$200 - DDoS**: Evolution of DoS with distributed sources
- **$300 - XSS**: Common web vulnerability
- **$400 - CSRF**: More complex web attack requiring understanding of sessions
- **$500 - APT**: Strategic, long-term threat actor concept

**Teaching Tips**:
- Use real-world examples (recent DDoS attacks in news)
- Explain XSS with simple example: stealing cookies via injected JavaScript
- Emphasize APT as nation-state or organized crime level threat

### 3. Security Tools
**Target Audience**: Security professionals, IT administrators

- **$100 - IDS**: Passive monitoring tool
- **$200 - IPS**: Active defense (builds on IDS)
- **$300 - SIEM**: Centralized logging and correlation
- **$400 - WAF**: Specialized firewall for web applications
- **$500 - SOAR**: Newest category, automation and orchestration

**Teaching Tips**:
- Compare IDS vs IPS (detective vs. detective + police)
- SIEM is the "brain" that correlates all security data
- SOAR represents the future of security operations

### 4. Compliance & Standards
**Target Audience**: GRC professionals, managers, auditors

- **$100 - GDPR**: Widely known, affects any EU business
- **$200 - PCI DSS**: Anyone handling credit cards
- **$300 - HIPAA**: Healthcare specific, US-based
- **$400 - NIST**: Government and framework basis
- **$500 - ISO 27001**: International certification standard

**Teaching Tips**:
- Emphasize regulatory penalties (GDPR fines can be massive)
- PCI DSS has 12 requirements - mention forensics after breach
- ISO 27001 is voluntary but shows commitment to security

### 5. Advanced Topics (Hardest)
**Target Audience**: Security architects, advanced practitioners

- **$100 - IAM**: Foundation of access control
- **$200 - EDR**: Next-gen antivirus replacement
- **$300 - CASB**: Cloud security broker concept
- **$400 - ZTNA**: Zero trust architecture principle
- **$500 - OSINT**: Intelligence gathering methodology

**Teaching Tips**:
- IAM is moving toward identity-centric security
- EDR vs traditional AV: behavioral vs signature-based
- ZTNA: "Never trust, always verify" - no implicit trust
- OSINT: Legal reconnaissance using public information

## Scoring Guidelines

### Point Awards
- **Exact Answer**: Full points (e.g., says exact acronym expansion)
- **Substantially Correct**: 75% of points (e.g., gets concept right but words slightly off)
- **Partial Credit**: 50% of points (e.g., gets some words but misses key part)
- **Incorrect**: No points or -100 (instructor's discretion)

### Scoring Strategies
1. **Encouraging**: Award partial credit liberally to keep engagement high
2. **Competitive**: Only award full points for exact answers
3. **Educational**: Award points for correct explanation even if acronym expansion is slightly off

## Time Management

### Full Game (60-90 minutes)
- Introduction: 5 minutes
- Game play: 50-70 minutes (25 questions × 2-3 minutes each)
- Wrap-up and discussion: 10-15 minutes

### Abbreviated Game (30-45 minutes)
- Play only $100-$300 rows (15 questions)
- Or select 2-3 categories only

### Quick Review (15-20 minutes)
- Play one category completely
- Focus on most relevant category for your audience

## Discussion Points

### Post-Game Debrief
1. Which acronyms were most familiar? Why?
2. Which acronyms do you encounter in your daily work?
3. What surprised you about the explanations?
4. Which security concepts need more training?

### Extension Activities
1. Have teams create their own acronym questions
2. Research recent breaches related to the acronyms
3. Map acronyms to your organization's security stack
4. Create action items: What should we implement?

## Common Questions & Answers

**Q: What if teams tie?**
A: Use sudden death - ask tiebreaker questions until one team gets it right.

**Q: Can teams challenge answers?**
A: Yes, instructor has final say. Use explanations on flip cards to justify.

**Q: What if a card is accidentally marked as used?**
A: Click "Reset Game" or refresh the page (scores will be lost unless manually tracked).

**Q: How do I adjust difficulty?**
A: For beginners, allow longer discussion time and provide hints. For experts, add time pressure.

## Troubleshooting

### Technical Issues
- **Cards not flipping**: Clear browser cache and reload
- **Modal won't close**: Click outside the modal or press ESC (if implemented)
- **Layout issues on mobile**: Rotate to landscape mode

### Gameplay Issues
- **Teams finishing too quickly**: Add "Daily Doubles" or require explanation
- **One team dominating**: Implement catch-up rules (wrong answers worth more negative points for leader)
- **Low engagement**: Use buzzer mode instead of turn-based

## Customization Tips

To modify questions:
1. Open the HTML file in a text editor
2. Find the `questions` object in the JavaScript section
3. Modify the `question`, `answer`, or `explanation` fields
4. Keep the structure consistent (value, question, answer, explanation)

Example:
```javascript
{
    value: 100,
    question: "What does NEW stand for?",
    answer: "New Example Word",
    explanation: "This is a custom explanation."
}
```

## Additional Resources

### For Further Learning
- **NIST Glossary**: Comprehensive security terms
- **SANS Glossary**: Practical security definitions
- **CISA Cybersecurity Resources**: Government training materials

### Related Training Materials
- Cybersecurity awareness presentations
- Hands-on labs for security tools
- Compliance framework workshops

## Assessment Ideas

### Learning Objectives Met
After playing, participants should be able to:
1. ✓ Recognize 25 common cybersecurity acronyms
2. ✓ Explain the purpose of each security concept
3. ✓ Differentiate between similar terms (IDS vs IPS, DoS vs DDoS)
4. ✓ Identify which tools/standards apply to their role

### Follow-Up Assessment
- Quiz on acronyms one week later (retention check)
- Ask participants to identify acronyms in security articles
- Practical exercise: map acronyms to actual security incidents

## Facilitator's Checklist

### Before the Session
- [ ] Test the game on the presentation system
- [ ] Decide on team composition
- [ ] Print score sheets (backup) if needed
- [ ] Prepare prizes or certificates (optional)
- [ ] Review all answers and explanations
- [ ] Plan discussion questions

### During the Session
- [ ] Explain rules clearly (5 minutes)
- [ ] Keep time - move game along at good pace
- [ ] Encourage participation from all team members
- [ ] Provide hints if teams are stuck
- [ ] Note which topics cause confusion

### After the Session
- [ ] Debrief and discuss challenging questions
- [ ] Collect feedback on game format
- [ ] Identify knowledge gaps for future training
- [ ] Share additional resources
- [ ] Schedule follow-up if needed

## Success Metrics

### Engagement Indicators
- All team members participating
- Energetic discussion during answer periods
- Teams asking follow-up questions
- Participants referencing game in later discussions

### Learning Indicators
- Improved scores in later rounds
- Participants making connections between concepts
- Teams explaining answers beyond the acronym expansion
- Follow-up questions showing deeper curiosity

---

## Quick Reference: Answer Key

### Basic Security
1. VPN = Virtual Private Network
2. SSL = Secure Sockets Layer
3. MFA = Multi-Factor Authentication
4. AES = Advanced Encryption Standard
5. PKI = Public Key Infrastructure

### Threats & Attacks
1. DoS = Denial of Service
2. DDoS = Distributed Denial of Service
3. XSS = Cross-Site Scripting
4. CSRF = Cross-Site Request Forgery
5. APT = Advanced Persistent Threat

### Security Tools
1. IDS = Intrusion Detection System
2. IPS = Intrusion Prevention System
3. SIEM = Security Information and Event Management
4. WAF = Web Application Firewall
5. SOAR = Security Orchestration, Automation and Response

### Compliance & Standards
1. GDPR = General Data Protection Regulation
2. PCI DSS = Payment Card Industry Data Security Standard
3. HIPAA = Health Insurance Portability and Accountability Act
4. NIST = National Institute of Standards and Technology
5. ISO 27001 = International Organization for Standardization 27001

### Advanced Topics
1. IAM = Identity and Access Management
2. EDR = Endpoint Detection and Response
3. CASB = Cloud Access Security Broker
4. ZTNA = Zero Trust Network Access
5. OSINT = Open Source Intelligence

---

**Version**: 1.0
**Last Updated**: October 2025
**Author**: Cybersecurity Training Team
**Contact**: For questions or customization requests, consult your training coordinator