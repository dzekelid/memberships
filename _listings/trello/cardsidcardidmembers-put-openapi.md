---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Cards Members
  description: Put cards members.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/memberships:
    get:
      summary: Get Boards Memberships
      description: Get boards memberships.
      operationId: getBoardsMembershipsByIdBoard
      x-api-path-slug: boardsidboardmemberships-get
      parameters:
      - in: query
        name: filter
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
  /boards/{idBoard}/memberships/{idMembership}:
    get:
      summary: Get Boards Memberships
      description: Get boards memberships.
      operationId: getBoardsMembershipsByIdBoardByIdMembership
      x-api-path-slug: boardsidboardmembershipsidmembership-get
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMembership
        description: idMembership
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
    put:
      summary: Put Boards Memberships
      description: Put boards memberships.
      operationId: updateBoardsMembershipsByIdBoardByIdMembership
      x-api-path-slug: boardsidboardmembershipsidmembership-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Memberships to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMembership
        description: idMembership
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
  /organizations/{idOrg}/memberships:
    get:
      summary: Get Organizations Memberships
      description: Get organizations memberships.
      operationId: getOrganizationsMembershipsByIdOrg
      x-api-path-slug: organizationsidorgmemberships-get
      parameters:
      - in: query
        name: filter
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Memberships
  /organizations/{idOrg}/memberships/{idMembership}:
    get:
      summary: Get Organizations Memberships
      description: Get organizations memberships.
      operationId: getOrganizationsMembershipsByIdOrgByIdMembership
      x-api-path-slug: organizationsidorgmembershipsidmembership-get
      parameters:
      - in: path
        name: idMembership
        description: idMembership
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Memberships
    put:
      summary: Put Organizations Memberships
      description: Put organizations memberships.
      operationId: updateOrganizationsMembershipsByIdOrgByIdMembership
      x-api-path-slug: organizationsidorgmembershipsidmembership-put
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations Memberships to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMembership
        description: idMembership
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Memberships
  /boards/{idBoard}/members:
    get:
      summary: Get Boards Members
      description: Get boards members.
      operationId: getBoardsMembersByIdBoard
      x-api-path-slug: boardsidboardmembers-get
      parameters:
      - in: query
        name: activity
        description: true or false ; works for premium organizations only
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: filter
        description: 'One of: admins, all, none, normal or owners'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
    put:
      summary: Put Boards Members
      description: Put boards members.
      operationId: updateBoardsMembersByIdBoard
      x-api-path-slug: boardsidboardmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
  /boards/{idBoard}/members/{filter}:
    get:
      summary: Get Boards Members Filter
      description: Get boards members filter.
      operationId: getBoardsMembersByIdBoardByFilter
      x-api-path-slug: boardsidboardmembersfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
      - Filter
  /boards/{idBoard}/members/{idMember}:
    delete:
      summary: Delete Boards Members
      description: Delete boards members.
      operationId: deleteBoardsMembersByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmember-delete
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
    put:
      summary: Put Boards Members
      description: Put boards members.
      operationId: updateBoardsMembersByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmember-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
  /boards/{idBoard}/members/{idMember}/cards:
    get:
      summary: Get Boards Members Cards
      description: Get boards members cards.
      operationId: getBoardsMembersCardsByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmembercards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: list
        description: true or false
      - in: query
        name: list_fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
      - Cards
  /cards/{idCard}/idMembers:
    post:
      summary: Post Cards Members
      description: Post cards members.
      operationId: addCardsIdMembersByIdCard
      x-api-path-slug: cardsidcardidmembers-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Members to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Members
    put:
      summary: Put Cards Members
      description: Put cards members.
      operationId: updateCardsIdMembersByIdCard
      x-api-path-slug: cardsidcardidmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Members
  /cards/{idCard}/idMembers/{idMember}:
    delete:
      summary: Delete Cards Members
      description: Delete cards members.
      operationId: deleteCardsIdMembersByIdCardByIdMember
      x-api-path-slug: cardsidcardidmembersidmember-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Members
  /cards/{idCard}/members:
    get:
      summary: Get Cards Members
      description: Get cards members.
      operationId: getCardsMembersByIdCard
      x-api-path-slug: cardsidcardmembers-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Members
  /members/{idMember}:
    get:
      summary: Get Members
      description: Get members.
      operationId: getMembersByIdMember
      x-api-path-slug: membersidmember-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_display
        description: true or false
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: action_before
        description: A date, or null
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: action_since
        description: A date, null or lastView
      - in: query
        name: boardBackgrounds
        description: 'One of: all, custom, default, none or premium'
      - in: query
        name: boards
        description: 'all or a comma-separated list of: closed, members, open, organization,
          pinned, public, starred or unpinned'
      - in: query
        name: boardsInvited
        description: 'all or a comma-separated list of: closed, members, open, organization,
          pinned, public, starred or unpinned'
      - in: query
        name: boardsInvited_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: boardStars
        description: true or false
      - in: query
        name: board_actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: board_actions_display
        description: true or false
      - in: query
        name: board_actions_entities
        description: true or false
      - in: query
        name: board_actions_format
        description: 'One of: count, list or minimal'
      - in: query
        name: board_actions_limit
        description: a number from 0 to 1000
      - in: query
        name: board_actions_since
        description: A date, null or lastView
      - in: query
        name: board_action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: board_lists
        description: 'One of: all, closed, none or open'
      - in: query
        name: board_memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: board_organization
        description: true or false
      - in: query
        name: board_organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: cards
        description: 'One of: all, closed, none, open or visible'
      - in: query
        name: card_attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: card_attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: card_members
        description: true or false
      - in: query
        name: card_member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: card_stickers
        description: true or false
      - in: query
        name: customBoardBackgrounds
        description: 'One of: all or none'
      - in: query
        name: customEmoji
        description: 'One of: all or none'
      - in: query
        name: customStickers
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: notifications
        description: 'all or a comma-separated list of: addAdminToBoard, addAdminToOrganization,
          addedAttachmentToCard, addedMemberToCard, addedToBoard, addedToCard, addedToOrganization,
          cardDueSoon, changeCard, closeBoard, commentCard, createdCard, declinedInvitationToBoard,
          declinedInvitationToOrganization, invitedToBoard, invitedToOrganization,
          makeAdminOfBoard, makeAdminOfOrganization, memberJoinedTrello, mentionedOnCard,
          removedFromBoard, removedFromCard, removedFromOrganization, removedMemberFromCard,
          unconfirmedInvitedToBoard, unconfirmedInvitedToOrganization or updateCheckItemStateOnCard'
      - in: query
        name: notifications_display
        description: true or false
      - in: query
        name: notifications_entities
        description: true or false
      - in: query
        name: notifications_limit
        description: a number from 1 to 1000
      - in: query
        name: notification_before
        description: An id, or null
      - in: query
        name: notification_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator,
          type or unread'
      - in: query
        name: notification_memberCreator
        description: true or false
      - in: query
        name: notification_memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: notification_since
        description: An id, or null
      - in: query
        name: organizations
        description: 'One of: all, members, none or public'
      - in: query
        name: organizationsInvited
        description: 'One of: all, members, none or public'
      - in: query
        name: organizationsInvited_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: organization_paid_account
        description: true or false
      - in: query
        name: paid_account
        description: true or false
      - in: query
        name: savedSearches
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      - in: query
        name: tokens
        description: 'One of: all or none'
      responses:
        200:
          description: OK
      tags:
      - Members
    put:
      summary: Put Members
      description: Put members.
      operationId: updateMembersByIdMember
      x-api-path-slug: membersidmember-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
  /members/{idMember}/actions:
    get:
      summary: Get Members Actions
      description: Get members actions.
      operationId: getMembersActionsByIdMember
      x-api-path-slug: membersidmemberactions-get
      parameters:
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: display
        description: true or false
      - in: query
        name: entities
        description: true or false
      - in: query
        name: fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: format
        description: 'One of: count, list or minimal'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: idModels
        description: Only return actions related to these model ids
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 0 to 1000
      - in: query
        name: member
        description: true or false
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: page
        description: Page * limit must be less than 1000
      - in: query
        name: since
        description: A date, null or lastView
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Actions
  /members/{idMember}/avatar:
    post:
      summary: Post Members Avatar
      description: Post members avatar.
      operationId: addMembersAvatarByIdMember
      x-api-path-slug: membersidmemberavatar-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Avatar to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Avatar
  /members/{idMember}/avatarSource:
    put:
      summary: Put Members Avatarsource
      description: Put members avatarsource.
      operationId: updateMembersAvatarSourceByIdMember
      x-api-path-slug: membersidmemberavatarsource-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Avatar Source to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Avatarsource
  /members/{idMember}/bio:
    put:
      summary: Put Members Bio
      description: Put members bio.
      operationId: updateMembersBioByIdMember
      x-api-path-slug: membersidmemberbio-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Bio to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Bio
  /members/{idMember}/boardBackgrounds:
    get:
      summary: Get Members Boardbackgrounds
      description: Get members boardbackgrounds.
      operationId: getMembersBoardBackgroundsByIdMember
      x-api-path-slug: membersidmemberboardbackgrounds-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all, custom, default, none or premium'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
    post:
      summary: Post Members Boardbackgrounds
      description: Post members boardbackgrounds.
      operationId: addMembersBoardBackgroundsByIdMember
      x-api-path-slug: membersidmemberboardbackgrounds-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Backgrounds to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
  /members/{idMember}/boardBackgrounds/{idBoardBackground}:
    delete:
      summary: Delete Members Boardbackgrounds Boardbackground
      description: Delete members boardbackgrounds boardbackground.
      operationId: deleteMembersBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmemberboardbackgroundsidboardbackground-delete
      parameters:
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
      - Boardbackground
    get:
      summary: Get Members Boardbackgrounds Boardbackground
      description: Get members boardbackgrounds boardbackground.
      operationId: getMembersBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmemberboardbackgroundsidboardbackground-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: brightness, fullSizeUrl, scaled
          or tile'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
      - Boardbackground
    put:
      summary: Put Members Boardbackgrounds Boardbackground
      description: Put members boardbackgrounds boardbackground.
      operationId: updateMembersBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmemberboardbackgroundsidboardbackground-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Backgrounds to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
      - Boardbackground
  /members/{idMember}/boardStars:
    get:
      summary: Get Members Boardstars
      description: Get members boardstars.
      operationId: getMembersBoardStarsByIdMember
      x-api-path-slug: membersidmemberboardstars-get
      parameters:
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
    post:
      summary: Post Members Boardstars
      description: Post members boardstars.
      operationId: addMembersBoardStarsByIdMember
      x-api-path-slug: membersidmemberboardstars-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
  /members/{idMember}/boardStars/{idBoardStar}:
    delete:
      summary: Delete Members Boardstars
      description: Delete members boardstars.
      operationId: deleteMembersBoardStarsByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstar-delete
      parameters:
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
    get:
      summary: Get Members Boardstars
      description: Get members boardstars.
      operationId: getMembersBoardStarsByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstar-get
      parameters:
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
    put:
      summary: Put Members Boardstars
      description: Put members boardstars.
      operationId: updateMembersBoardStarsByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstar-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
  /members/{idMember}/boardStars/{idBoardStar}/idBoard:
    put:
      summary: Put Members Boardstars Board
      description: Put members boardstars board.
      operationId: updateMembersBoardStarsIdBoardByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstaridboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars Id Board to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
      - Board
  /members/{idMember}/boardStars/{idBoardStar}/pos:
    put:
      summary: Put Members Boardstars Pos
      description: Put members boardstars pos.
      operationId: updateMembersBoardStarsPosByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstarpos-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars Pos to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
      - Pos
  /members/{idMember}/boards:
    get:
      summary: Get Members Boards
      description: Get members boards.
      operationId: getMembersBoardsByIdMember
      x-api-path-slug: membersidmemberboards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_format
        description: 'One of: count, list or minimal'
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: actions_since
        description: A date, null or lastView
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: closed, members, open, organization,
          pinned, public, starred or unpinned'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: lists
        description: 'One of: all, closed, none or open'
      - in: query
        name: memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: organization
        description: true or false
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boards
  /members/{idMember}/boards/{filter}:
    get:
      summary: Get Members Boards Filter
      description: Get members boards filter.
      operationId: getMembersBoardsByIdMemberByFilter
      x-api-path-slug: membersidmemberboardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boards
      - Filter
  /members/{idMember}/boardsInvited:
    get:
      summary: Get Members Boardsinvited
      description: Get members boardsinvited.
      operationId: getMembersBoardsInvitedByIdMember
      x-api-path-slug: membersidmemberboardsinvited-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardsinvited
  /members/{idMember}/boardsInvited/{field}:
    get:
      summary: Get Members Boardsinvited Field
      description: Get members boardsinvited field.
      operationId: getMembersBoardsInvitedByIdMemberByField
      x-api-path-slug: membersidmemberboardsinvitedfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardsinvited
      - Field
  /members/{idMember}/cards:
    get:
      summary: Get Members Cards
      description: Get members cards.
      operationId: getMembersCardsByIdMember
      x-api-path-slug: membersidmembercards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 1000
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: since
        description: A date, or null
      - in: query
        name: stickers
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Cards
  /members/{idMember}/cards/{filter}:
    get:
      summary: Get Members Cards Filter
      description: Get members cards filter.
      operationId: getMembersCardsByIdMemberByFilter
      x-api-path-slug: membersidmembercardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Cards
      - Filter
  /members/{idMember}/customBoardBackgrounds:
    get:
      summary: Get Members Customboardbackgrounds
      description: Get members customboardbackgrounds.
      operationId: getMembersCustomBoardBackgroundsByIdMember
      x-api-path-slug: membersidmembercustomboardbackgrounds-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all or none'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
    post:
      summary: Post Members Customboardbackgrounds
      description: Post members customboardbackgrounds.
      operationId: addMembersCustomBoardBackgroundsByIdMember
      x-api-path-slug: membersidmembercustomboardbackgrounds-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Custom Board Backgrounds to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
  /members/{idMember}/customBoardBackgrounds/{idBoardBackground}:
    delete:
      summary: Delete Members Customboardbackgrounds Boardbackground
      description: Delete members customboardbackgrounds boardbackground.
      operationId: deleteMembersCustomBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmembercustomboardbackgroundsidboardbackground-delete
      parameters:
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
      - Boardbackground
    get:
      summary: Get Members Customboardbackgrounds Boardbackground
      description: Get members customboardbackgrounds boardbackground.
      operationId: getMembersCustomBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmembercustomboardbackgroundsidboardbackground-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: brightness, fullSizeUrl, scaled
          or tile'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
      - Boardbackground
    put:
      summary: Put Members Customboardbackgrounds Boardbackground
      description: Put members customboardbackgrounds boardbackground.
      operationId: updateMembersCustomBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmembercustomboardbackgroundsidboardbackground-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Custom Board Backgrounds to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
      - Boardbackground
  /members/{idMember}/customEmoji:
    get:
      summary: Get Members Customemoji
      description: Get members customemoji.
      operationId: getMembersCustomEmojiByIdMember
      x-api-path-slug: membersidmembercustomemoji-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all or none'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customemoji
    post:
      summary: Post Members Customemoji
      description: Post members customemoji.
      operationId: addMembersCustomEmojiByIdMember
      x-api-path-slug: membersidmembercustomemoji-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Custom Emoji to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customemoji
  /members/{idMember}/customEmoji/{idCustomEmoji}:
    get:
      summary: Get Members Customemoji Customemoji
      description: Get members customemoji customemoji.
      operationId: getMembersCustomEmojiByIdMemberByIdCustomEmoji
      x-api-path-slug: membersidmembercustomemojiidcustomemoji-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: name or url'
      - in: path
        name: idCustomEmoji
        description: idCustomEmoji
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customemoji
      - Customemoji
  /members/{idMember}/customStickers:
    get:
      summary: Get Members Customstickers
      description: Get members customstickers.
      operationId: getMembersCustomStickersByIdMember
      x-api-path-slug: membersidmembercustomstickers-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all or none'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customstickers
    post:
      summary: Post Members Customstickers
      description: Post members customstickers.
      operationId: addMembersCustomStickersByIdMember
      x-api-path-slug: membersidmembercustomstickers-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Custom Stickers to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customstickers
  /members/{idMember}/customStickers/{idCustomSticker}:
    delete:
      summary: Delete Members Customstickers Customsticker
      description: Delete members customstickers customsticker.
      operationId: deleteMembersCustomStickersByIdMemberByIdCustomSticker
      x-api-path-slug: membersidmembercustomstickersidcustomsticker-delete
      parameters:
      - in: path
        name: idCustomSticker
        description: idCustomSticker
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customstickers
      - Customsticker
    get:
      summary: Get Members Customstickers Customsticker
      description: Get members customstickers customsticker.
      operationId: getMembersCustomStickersByIdMemberByIdCustomSticker
      x-api-path-slug: membersidmembercustomstickersidcustomsticker-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: scaled or url'
      - in: path
        name: idCustomSticker
        description: idCustomSticker
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customstickers
      - Customsticker
  /members/{idMember}/deltas:
    get:
      summary: Get Members Deltas
      description: Get members deltas.
      operationId: getMembersDeltasByIdMember
      x-api-path-slug: membersidmemberdeltas-get
      parameters:
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: ixLastUpdate
        description: a number from -1 to Infinity
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: tags
        description: A valid tag for subscribing
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Deltas
  /members/{idMember}/fullName:
    put:
      summary: Put Members Fullname
      description: Put members fullname.
      operationId: updateMembersFullNameByIdMember
      x-api-path-slug: membersidmemberfullname-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Full Name to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Fullname
  /members/{idMember}/initials:
    put:
      summary: Put Members Initials
      description: Put members initials.
      operationId: updateMembersInitialsByIdMember
      x-api-path-slug: membersidmemberinitials-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Initials to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Initials
  /members/{idMember}/notifications:
    get:
      summary: Get Members Notifications
      description: Get members notifications.
      operationId: getMembersNotificationsByIdMember
      x-api-path-slug: membersidmembernotifications-get
      parameters:
      - in: query
        name: before
        description: An id, or null
      - in: query
        name: display
        description: true or false
      - in: query
        name: entities
        description: true or false
      - in: query
        name: fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator,
          type or unread'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: addAdminToBoard, addAdminToOrganization,
          addedAttachmentToCard, addedMemberToCard, addedToBoard, addedToCard, addedToOrganization,
          cardDueSoon, changeCard, closeBoard, commentCard, createdCard, declinedInvitationToBoard,
          declinedInvitationToOrganization, invitedToBoard, invitedToOrganization,
          makeAdminOfBoard, makeAdminOfOrganization, memberJoinedTrello, mentionedOnCard,
          removedFromBoard, removedFromCard, removedFromOrganization, removedMemberFromCard,
          unconfirmedInvitedToBoard, unconfirmedInvitedToOrganization or updateCheckItemStateOnCard'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 1000
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: page
        description: a number from 0 to 100
      - in: query
        name: read_filter
        description: 'One of: all, read or unread'
      - in: query
        name: since
        description: An id, or null
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Notifications
  /members/{idMember}/notifications/{filter}:
    get:
      summary: Get Members Notifications Filter
      description: Get members notifications filter.
      operationId: getMembersNotificationsByIdMemberByFilter
      x-api-path-slug: membersidmembernotificationsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Notifications
      - Filter
  /members/{idMember}/oneTimeMessagesDismissed:
    post:
      summary: Post Members Onetimemessagesdismissed
      description: Post members onetimemessagesdismissed.
      operationId: addMembersOneTimeMessagesDismissedByIdMember
      x-api-path-slug: membersidmemberonetimemessagesdismissed-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members One Time Messages Dismissed to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Onetimemessagesdismissed
  /members/{idMember}/organizations:
    get:
      summary: Get Members Organizations
      description: Get members organizations.
      operationId: getMembersOrganizationsByIdMember
      x-api-path-slug: membersidmemberorganizations-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: filter
        description: 'One of: all, members, none or public'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: paid_account
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizations
  /members/{idMember}/organizations/{filter}:
    get:
      summary: Get Members Organizations Filter
      description: Get members organizations filter.
      operationId: getMembersOrganizationsByIdMemberByFilter
      x-api-path-slug: membersidmemberorganizationsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizations
      - Filter
  /members/{idMember}/organizationsInvited:
    get:
      summary: Get Members Organizationsinvited
      description: Get members organizationsinvited.
      operationId: getMembersOrganizationsInvitedByIdMember
      x-api-path-slug: membersidmemberorganizationsinvited-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizationsinvited
  /members/{idMember}/organizationsInvited/{field}:
    get:
      summary: Get Members Organizationsinvited Field
      description: Get members organizationsinvited field.
      operationId: getMembersOrganizationsInvitedByIdMemberByField
      x-api-path-slug: membersidmemberorganizationsinvitedfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizationsinvited
      - Field
  /members/{idMember}/prefs/colorBlind:
    put:
      summary: Put Members Preferences Colorblind
      description: Put members preferences colorblind.
      operationId: updateMembersPrefsColorBlindByIdMember
      x-api-path-slug: membersidmemberprefscolorblind-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Color Blind to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Preferences
      - Colorblind
  /members/{idMember}/prefs/locale:
    put:
      summary: Put Members Preferences Locale
      description: Put members preferences locale.
      operationId: updateMembersPrefsLocaleByIdMember
      x-api-path-slug: membersidmemberprefslocale-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Locale to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Preferences
      - Locale
  /members/{idMember}/prefs/minutesBetweenSummaries:
    put:
      summary: Put Members Preferences Minutesbetweensummaries
      description: Put members preferences minutesbetweensummaries.
      operationId: updateMembersPrefsMinutesBetweenSummariesByIdMember
      x-api-path-slug: membersidmemberprefsminutesbetweensummaries-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Minutes Between Summaries to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Preferences
      - Minutesbetweensummaries
  /members/{idMember}/savedSearches:
    get:
      summary: Get Members Savedsearches
      description: Get members savedsearches.
      operationId: getMembersSavedSearchesByIdMember
      x-api-path-slug: membersidmembersavedsearches-get
      parameters:
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
    post:
      summary: Post Members Savedsearches
      description: Post members savedsearches.
      operationId: addMembersSavedSearchesByIdMember
      x-api-path-slug: membersidmembersavedsearches-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Saved Searches to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
  /members/{idMember}/savedSearches/{idSavedSearch}:
    delete:
      summary: Delete Members Savedsearches Savedsearch
      description: Delete members savedsearches savedsearch.
      operationId: deleteMembersSavedSearchesByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearch-delete
      parameters:
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
    get:
      summary: Get Members Savedsearches Savedsearch
      description: Get members savedsearches savedsearch.
      operationId: getMembersSavedSearchesByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearch-get
      parameters:
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
    put:
      summary: Put Members Savedsearches Savedsearch
      description: Put members savedsearches savedsearch.
      operationId: updateMembersSavedSearchesByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearch-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Saved Searches to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
  /members/{idMember}/savedSearches/{idSavedSearch}/name:
    put:
      summary: Put Members Savedsearches Savedsearch Name
      description: Put members savedsearches savedsearch name.
      operationId: updateMembersSavedSearchesNameByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearchname-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Saved Searches Name to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
      - Name
  /members/{idMember}/savedSearches/{idSavedSearch}/pos:
    put:
      summary: Put Members Savedsearches Savedsearch Pos
      description: Put members savedsearches savedsearch pos.
      operationId: updateMembersSavedSearchesPosByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearchpos-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Saved Searches Pos to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
      - Pos
  /members/{idMember}/savedSearches/{idSavedSearch}/query:
    put:
      summary: Put Members Savedsearches Savedsearch Query
      description: Put members savedsearches savedsearch query.
      operationId: updateMembersSavedSearchesQueryByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearchquery-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Saved Searches Query to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
      - Query
  /members/{idMember}/tokens:
    get:
      summary: Get Members Tokens
      description: Get members tokens.
      operationId: getMembersTokensByIdMember
      x-api-path-slug: membersidmembertokens-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all or none'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Tokens
  /members/{idMember}/username:
    put:
      summary: Put Members Username
      description: Put members username.
      operationId: updateMembersUsernameByIdMember
      x-api-path-slug: membersidmemberusername-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Username to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Username
  /members/{idMember}/{field}:
    get:
      summary: Get Members Field
      description: Get members field.
      operationId: getMembersByIdMemberByField
      x-api-path-slug: membersidmemberfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Field
  /organizations/{idOrg}/members:
    get:
      summary: Get Organizations Members
      description: Get organizations members.
      operationId: getOrganizationsMembersByIdOrg
      x-api-path-slug: organizationsidorgmembers-get
      parameters:
      - in: query
        name: activity
        description: true or false ; works for premium organizations only
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: filter
        description: 'One of: admins, all, none, normal or owners'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
    put:
      summary: Put Organizations Members
      description: Put organizations members.
      operationId: updateOrganizationsMembersByIdOrg
      x-api-path-slug: organizationsidorgmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
  /organizations/{idOrg}/members/{filter}:
    get:
      summary: Get Organizations Members Filter
      description: Get organizations members filter.
      operationId: getOrganizationsMembersByIdOrgByFilter
      x-api-path-slug: organizationsidorgmembersfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
      - Filter
  /organizations/{idOrg}/members/{idMember}:
    delete:
      summary: Delete Organizations Members
      description: Delete organizations members.
      operationId: deleteOrganizationsMembersByIdOrgByIdMember
      x-api-path-slug: organizationsidorgmembersidmember-delete
      parameters:
      - in: path
        name: idMember
        description: idMember
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
    put:
      summary: Put Organizations Members
      description: Put organizations members.
      operationId: updateOrganizationsMembersByIdOrgByIdMember
      x-api-path-slug: organizationsidorgmembersidmember-put
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
  /organizations/{idOrg}/members/{idMember}/all:
    delete:
      summary: Delete Organizations Members All
      description: Delete organizations members all.
      operationId: deleteOrganizationsMembersAllByIdOrgByIdMember
      x-api-path-slug: organizationsidorgmembersidmemberall-delete
      parameters:
      - in: path
        name: idMember
        description: idMember
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
  /organizations/{idOrg}/members/{idMember}/cards:
    get:
      summary: Get Organizations Members Cards
      description: Get organizations members cards.
      operationId: getOrganizationsMembersCardsByIdOrgByIdMember
      x-api-path-slug: organizationsidorgmembersidmembercards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idMember
        description: idMember
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: list
        description: true or false
      - in: query
        name: list_fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
      - Cards
  /organizations/{idOrg}/members/{idMember}/deactivated:
    put:
      summary: Put Organizations Members Deactivated
      description: Put organizations members deactivated.
      operationId: updateOrganizationsMembersDeactivatedByIdOrgByIdMember
      x-api-path-slug: organizationsidorgmembersidmemberdeactivated-put
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations Members Deactivated to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
      - Deactivated
  /search/members:
    get:
      summary: Get Search Members
      description: Get search members.
      operationId: getSearchMembers
      x-api-path-slug: searchmembers-get
      parameters:
      - in: query
        name: idBoard
        description: An id, or null
      - in: query
        name: idOrganization
        description: An id, or null
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 20
      - in: query
        name: onlyOrgMembers
        description: A boolean
      - in: query
        name: query
        description: a string with a length from 1 to 16384
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Search
      - Members
  /actions/{idAction}/member:
    get:
      summary: Get Actions Member
      description: Get actions member.
      operationId: getActionsMemberByIdAction
      x-api-path-slug: actionsidactionmember-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Member
  /actions/{idAction}/member/{field}:
    get:
      summary: Get Actions Member Field
      description: Get actions member field.
      operationId: getActionsMemberByIdActionByField
      x-api-path-slug: actionsidactionmemberfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Member
      - Field
  /actions/{idAction}/memberCreator:
    get:
      summary: Get Actions Member Creator
      description: Get actions member creator.
      operationId: getActionsMemberCreatorByIdAction
      x-api-path-slug: actionsidactionmembercreator-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Member
      - Creator
  /actions/{idAction}/memberCreator/{field}:
    get:
      summary: Get Actions Member Creator Field
      description: Get actions member creator field.
      operationId: getActionsMemberCreatorByIdActionByField
      x-api-path-slug: actionsidactionmembercreatorfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Member
      - Creator
      - Field
  /cards/{idCard}/membersVoted/{idMember}:
    delete:
      summary: Delete Cards Membersvoted Member
      description: Delete cards membersvoted member.
      operationId: deleteCardsMembersVotedByIdCardByIdMember
      x-api-path-slug: cardsidcardmembersvotedidmember-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Membersvoted
      - Member
  /notifications/{idNotification}/member:
    get:
      summary: Get Notifications Notification Member
      description: Get notifications notification member.
      operationId: getNotificationsMemberByIdNotification
      x-api-path-slug: notificationsidnotificationmember-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
  /notifications/{idNotification}/member/{field}:
    get:
      summary: Get Notifications Notification Member Field
      description: Get notifications notification member field.
      operationId: getNotificationsMemberByIdNotificationByField
      x-api-path-slug: notificationsidnotificationmemberfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
      - Field
  /notifications/{idNotification}/memberCreator:
    get:
      summary: Get Notifications Notification Member Creator
      description: Get notifications notification member creator.
      operationId: getNotificationsMemberCreatorByIdNotification
      x-api-path-slug: notificationsidnotificationmembercreator-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
      - Creator
  /notifications/{idNotification}/memberCreator/{field}:
    get:
      summary: Get Notifications Notification Member Creator Field
      description: Get notifications notification member creator field.
      operationId: getNotificationsMemberCreatorByIdNotificationByField
      x-api-path-slug: notificationsidnotificationmembercreatorfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
      - Creator
      - Field
  /tokens/{token}/member:
    get:
      summary: Get Tokens Member
      description: Get tokens member.
      operationId: getTokensMemberByToken
      x-api-path-slug: tokenstokenmember-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Member
  /tokens/{token}/member/{field}:
    get:
      summary: Get Tokens Member Field
      description: Get tokens member field.
      operationId: getTokensMemberByTokenByField
      x-api-path-slug: tokenstokenmemberfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Member
      - Field
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---