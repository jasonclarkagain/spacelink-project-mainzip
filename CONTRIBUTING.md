# Contributing to SpaceLink

## Platform Values

SpaceLink is built on these core principles:
- **Free Speech**: Open dialogue while protecting minors
- **Privacy**: User data protection and anonymous options
- **Community**: Bringing people together with respect
- **Independence**: Alternative information sources
- **Safety**: Protecting vulnerable community members

## Development Guidelines

### Code Style
- Use TypeScript for all new code
- Follow existing naming conventions
- Add proper error handling
- Include JSDoc comments for functions
- Use meaningful variable names

### Database Changes
- Always use Drizzle migrations
- Never directly modify production database
- Test schema changes locally first
- Update shared/schema.ts for any table changes

### Security Requirements
- All adult content must be properly gated
- Validate all user inputs
- Use parameterized queries
- Implement proper authentication checks
- Review privacy implications

### Content Guidelines
- Respect free speech principles
- Protect minors from inappropriate content
- Support independent information sources
- Promote community safety and awareness
- Encourage respectful dialogue

## Pull Request Process

1. Fork the repository
2. Create feature branch: `git checkout -b feature/your-feature`
3. Make changes following guidelines above
4. Test thoroughly (auth, uploads, messaging)
5. Update documentation if needed
6. Submit pull request with detailed description

## Testing
- Test authentication flow
- Verify file upload/download
- Check adult content verification
- Test real-time messaging
- Validate API endpoints

## Feature Priorities

### High Priority
- Core social features (posts, messaging, profiles)
- Security and privacy tools
- Adult content protection
- Database performance

### Medium Priority
- New app marketplace widgets
- Additional video platform support
- Enhanced customization options
- Community moderation tools

### Low Priority
- Visual enhancements
- Additional themes
- Performance optimizations
- Analytics features

## Bug Reports

Include:
- Steps to reproduce
- Expected vs actual behavior
- Browser/environment details
- Screenshots if applicable
- Privacy considerations

## Community Standards

- Treat all contributors with respect
- Focus on constructive feedback
- Protect user privacy in discussions
- Support independent information sharing
- Maintain platform safety standards