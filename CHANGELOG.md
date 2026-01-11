# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.0] - 2025-01-11

### Added

- Initial release
- Full MCP server for Meta's Threads API
- Built on [meta-threads-sdk](https://github.com/MetaThreads/meta-threads-sdk) and [FastMCP](https://github.com/jlowin/fastmcp)
- Post management tools
  - `threads_create_post` - Create text posts
  - `threads_create_image_post` - Create image posts
  - `threads_create_video_post` - Create video posts
  - `threads_get_post` - Get post by ID
  - `threads_get_user_posts` - Get user's recent posts
  - `threads_delete_post` - Delete a post
  - `threads_get_publishing_limit` - Check publishing quota
- Reply management tools
  - `threads_reply_to_post` - Reply to a post
  - `threads_get_replies` - Get replies to a post
  - `threads_get_conversation` - Get full conversation thread
  - `threads_hide_reply` - Hide a reply
  - `threads_unhide_reply` - Unhide a reply
- Insights tools
  - `threads_get_media_insights` - Get post metrics
  - `threads_get_user_insights` - Get user-level metrics
- User tools
  - `threads_get_profile` - Get authenticated user's profile
- MCP prompts for content strategy
  - `reply_strategy` - Craft thoughtful replies
  - `content_ideas` - Generate content ideas
  - `analyze_engagement` - Analyze engagement metrics
- Flexible authentication
  - HTTP Authorization header (for SSE/HTTP transport)
  - Environment variables (for stdio/Claude Desktop)
- Full test suite with 92% coverage
