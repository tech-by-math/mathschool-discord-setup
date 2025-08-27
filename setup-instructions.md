# 🛠️ MathSchool Discord Server Setup Instructions

## Overview

This guide provides step-by-step instructions for setting up the MathSchool Discord server according to the recommended structure. Follow these instructions carefully to ensure proper functionality and permissions.

---

## 📋 Pre-Setup Checklist

### Requirements
- Discord server with Administrator permissions
- Access to Discord's Server Settings
- List of current students and their enrolled courses
- Staff list (Teachers, TAs, Tutors)

### Preparation
1. **Backup existing server** (if applicable)
2. **Plan implementation timing** (recommend during low activity periods)
3. **Notify community** about upcoming changes
4. **Prepare role assignments** spreadsheet

---

## 🎭 Phase 1: Role Creation

### Step 1: Create Staff Roles
Create these roles in order (higher roles have more permissions):

1. **Admin**
   - Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #FF0000; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>Red (#FF0000)
   - Permissions: Administrator
   - Hoist: Yes
   - Mentionable: No

2. **Teacher**
   - Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #9932CC; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>Purple (#9932CC)
   - Permissions: Manage Channels, Manage Messages, Kick Members, Mute Members
   - Hoist: Yes
   - Mentionable: Yes

3. **TA**
   - Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #0000FF; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>Blue (#0000FF)
   - Permissions: Manage Messages, Mute Members
   - Hoist: Yes
   - Mentionable: Yes

4. **Tutor**
   - Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #008000; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>Green (#008000)
   - Permissions: Manage Messages (in homework help only)
   - Hoist: Yes
   - Mentionable: Yes

### Step 2: Create Student Semester Roles

#### Current Semester Roles (Update year as needed)
Create these roles without special permissions:

**Computer Science Courses:**
- `2025-CS1` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #FF6B6B; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#FF6B6B)
- `2025-CS2` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #FF8E53; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#FF8E53)
- `2025-CS3` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #FF6B9D; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#FF6B9D)
- `2025-CS4` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #C44569; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#C44569)

**Mathematics Courses:**
- `2025-L1` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #4834D4; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#4834D4)
- `2025-L2` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #6C5CE7; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#6C5CE7)
- `2025-FunMath1` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #A55EEA; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#A55EEA)
- `2025-FunMath2` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #FD79A8; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#FD79A8)
- `2025-AMC8` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #00B894; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#00B894)
- `2025-AMC10` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #00CEC9; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#00CEC9)
- `2025-AMC12` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #81ECEC; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#81ECEC)
- `2025-AIME` (Color: <span style="display: inline-block; width: 16px; height: 16px; background-color: #74B9FF; border: 1px solid #000; vertical-align: middle; margin-right: 6px;"></span>#74B9FF)

#### Role Settings for Student Roles:
- Permissions: Default (@everyone permissions)
- Hoist: No
- Mentionable: Yes

---

## 🏗️ Phase 2: Channel Structure Creation

### Step 1: Global Community Channels

Create these channels in the main server area:

1. **#announcements**
   - Type: Text Channel
   - Permissions: 
     - @everyone: View Channel, Read Message History
     - Teachers/Admins: Send Messages, Manage Messages
   - Settings: Slowmode 10 minutes

2. **#general-chat**
   - Type: Text Channel
   - Permissions: Default
   - Settings: No slowmode

3. **#events**
   - Type: Text Channel
   - Permissions: Default
   - Settings: Slowmode 30 seconds

4. **#q-and-a**
   - Type: Text Channel
   - Permissions: Default
   - Settings: Slowmode 30 seconds

5. **#tech-support**
   - Type: Text Channel
   - Permissions: Default
   - Settings: No slowmode

### Step 2: Create Homework Help Category

1. **Create Category: "Homework Help"**
   - Position: After Global Community channels
   - Permissions: All students can view and participate

2. **#math-homework-help**
   - Type: Forum Channel
   - Parent Category: Homework Help
   - Available Tags:
     - `L1` (Color: Blue)
     - `L2` (Color: Purple)  
     - `FunMath1` (Color: Pink)
     - `FunMath2` (Color: Red)
     - `AMC8` (Color: Green)
     - `AMC10` (Color: Teal)
     - `AMC12` (Color: Yellow)
     - `AIME` (Color: Orange)
   - Default Sort: Latest Activity
   - Default Layout: List View

3. **#cs-homework-help**
   - Type: Forum Channel
   - Parent Category: Homework Help
   - Available Tags:
     - `CS1` (Color: Light Blue)
     - `CS2` (Color: Blue)
     - `CS3` (Color: Dark Blue)
     - `CS4` (Color: Purple)
   - Default Sort: Latest Activity
   - Default Layout: List View

### Step 3: Create Classroom Channels

#### Mathematics Classrooms
Create these as private text channels:

- `#l1-classroom`
- `#l2-classroom`  
- `#funmath1-classroom`
- `#funmath2-classroom`
- `#amc8-classroom`
- `#amc10-classroom`
- `#amc12-classroom`
- `#aime-classroom`

#### Computer Science Classrooms
- `#cs1-classroom`
- `#cs2-classroom`
- `#cs3-classroom`
- `#cs4-classroom`

#### Classroom Channel Permissions Template:
- **@everyone**: No access
- **Corresponding semester role** (e.g., 2025-CS1): View Channel, Send Messages, Read Message History
- **Teachers**: Full access
- **TAs**: Full access
- **Admins**: Full access

### Step 4: Staff Channels

Create Category: "Staff"
- Position: After all student channels
- Permissions: Staff roles only

1. **#teacher-lounge**
   - Type: Text Channel
   - Permissions: Teachers, Admins only

2. **#staff-announcements**
   - Type: Text Channel
   - Permissions: 
     - Teachers, TAs, Admins: View, React
     - Admins: Send Messages

3. **#materials-bank**
   - Type: Text Channel
   - Permissions: Teachers, TAs, Tutors, Admins

---

## ⚙️ Phase 3: Permission Configuration

### Forum Channel Permissions Setup

For both homework help forums:

1. **@everyone**:
   - View Channel: ✅
   - Send Messages in Threads: ✅
   - Create Public Threads: ✅
   - Send Messages: ❌ (Forum channels use threads)
   - Embed Links: ✅
   - Attach Files: ✅
   - Read Message History: ✅
   - Use External Emoji: ✅
   - Add Reactions: ✅

2. **Staff Roles (Teacher, TA, Tutor, Admin)**:
   - All above permissions: ✅
   - Manage Messages: ✅
   - Manage Threads: ✅
   - Mention Everyone: ✅

### Default Thread Settings
- **Auto-archive duration**: 1 week
- **Default thread slowmode**: 10 seconds
- **Require tag**: Yes (for homework help forums)

---

## 📌 Phase 4: Initial Content Setup

### Step 1: Pin Essential Messages

In **#announcements**:
1. Pin the Server Rules & Culture document
2. Pin a welcome message with server overview
3. Pin current semester important dates

In each **classroom channel**:
1. Pin a welcome message explaining the channel purpose
2. Pin homework submission guidelines
3. Pin class-specific resources/links

### Step 2: Set Up Forum Templates

For **#math-homework-help**:
```
**Problem Description:**
[Describe your problem here]

**What I've Tried:**
[Show your work and explain where you're stuck]

**Course/Level:**
[Use the appropriate tag: L1, L2, AMC8, etc.]

**Specific Question:**
[What exactly are you confused about?]
```

For **#cs-homework-help**:
```
**Assignment/Problem:**
[Describe what you're working on]

**Code So Far:**
```code
[Your current code here]
```

**Error Message (if any):**
[Copy any error messages here]

**Course Level:**
[Use the appropriate tag: CS1, CS2, CS3, CS4]

**What I've Tried:**
[Explain your debugging attempts]
```

---

## 👥 Phase 5: Member Management

### Step 1: Assign Staff Roles
1. Assign Admin roles to server administrators
2. Assign Teacher roles to course instructors  
3. Assign TA roles to teaching assistants
4. Assign Tutor roles to homework help moderators

### Step 2: Assign Student Roles

#### Bulk Role Assignment Process:
1. **Prepare spreadsheet** with Discord usernames and enrolled courses
2. **Use Discord bots** (like Carl-bot or Dyno) for bulk role assignments, or
3. **Manual assignment** through Server Settings > Members

#### Role Assignment Rules:
- Students can have **multiple semester roles** if enrolled in multiple courses
- **Remove old semester roles** at the end of each term
- **Add new roles** at the beginning of each semester

### Step 3: Onboarding New Members

Create an **#onboarding** process:
1. New members join with no roles initially
2. They react to get their appropriate course roles
3. Alternatively, staff manually assigns roles after verification

---

## 🔧 Phase 6: Bot Setup (Recommended)

### Essential Bots

1. **MEE6 or Carl-bot**
   - Auto-role assignment
   - Moderation commands
   - Welcome messages

2. **Ticket Tool or Ticket Buddy**
   - Private support tickets
   - Staff communication

3. **Poll Bot**
   - Course feedback
   - Event planning

### Bot Permissions
- Assign appropriate roles to bots
- Limit permissions to necessary functions only
- Regular permission audits

---

## 📊 Phase 7: Testing & Launch

### Pre-Launch Testing

1. **Test all channel permissions** with test accounts
2. **Verify role assignments** work correctly
3. **Test forum functionality** and tags
4. **Check staff permissions** in all areas
5. **Test bot functions** if applicable

### Soft Launch Process

1. **Invite staff first** for final testing
2. **Invite small group of students** for feedback
3. **Address any issues** discovered
4. **Full community migration**

### Launch Day Checklist

- [ ] All channels created and configured
- [ ] All roles assigned correctly  
- [ ] Welcome messages and rules posted
- [ ] Staff trained on new structure
- [ ] Announcement posted about new server structure
- [ ] Old channels archived (if applicable)
- [ ] Bot functions tested and working

---

## 🔄 Ongoing Maintenance

### Weekly Tasks
- Review flagged messages in homework help
- Update pinned messages as needed
- Check for inactive threads to archive

### Semester Tasks
- Update semester role years (2025 → 2026)
- Archive old classroom channels
- Create new channels for new courses
- Bulk role updates for continuing students

### Annual Tasks
- Server permission audit
- Channel structure review
- Community feedback collection
- Documentation updates

---

## 🆘 Troubleshooting

### Common Issues

**Students can't see homework help forums:**
- Check @everyone permissions on Homework Help category
- Verify forum channels inherit category permissions

**Classroom channels showing to wrong students:**
- Double-check semester role assignments
- Verify channel permission overrides

**Staff can't moderate properly:**
- Check role hierarchy (staff roles above student roles)
- Verify staff permissions in each channel

**Forum tags not working:**
- Ensure "Require Tag" is enabled
- Check tag permissions and colors

### Emergency Contacts
- Document admin contacts for urgent issues
- Have backup admin accounts configured
- Keep server backup/export updated

---

## 📚 Related Documentation

For complete server information and ongoing management:

- **[📋 Main Documentation](README.md)** - Complete server structure overview and design philosophy
- **[📜 Server Rules & Culture](server-rules-culture.md)** - Community guidelines and user onboarding
- **[🎭 Roles & Permissions](roles-and-permissions.md)** - Detailed role configuration and troubleshooting
- **[📊 Channel Management](channel-management.md)** - Ongoing moderation and community building

---

## 📞 Support

For questions about this setup:
- Review the [main documentation](README.md)
- Check Discord's official server setup guides
- Contact the server admin team
- Post in #tech-support for community help

---

*Last updated: [Current Date]*
*Version: 1.0*