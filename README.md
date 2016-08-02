# uber-mobile-rider-endpoints
Unofficial Documentation of Uber Endpoints (Rider)

Work in progress

**Possible Hosts:**


```
https://cn-dc1.uber.com 
https://cn.uber.com
```


**GET:**

| Path | Required Headers | Required Params |
|------|------------------|------------------|
| /rt/onboarding/dynamic-form/step/{driverUUID} | x-uber-token ||
| /rt/onboarding/signup | x-uber-device-language ||
| /rt/drivers/{driverUUID}/vault | x-uber-token ||
| /rt/onboarding/step/{partnerUuid} | x-uber-onboarding-variant <br /> x-uber-token ||
| /rt/onboarding/unified-step/{partnerUuid} | x-uber-onboarding-variant <br /> x-uber-token ||
| /rt/onboarding/dynamic-form/signup |||
| /rt/onboarding/dynamic-form/upgrade |||
| /rt/payment/payment_profiles/{id}/balance | x-uber-token ||
| /rt/payment/v2/payment_profiles | x-uber-token ||
| /rt/payment/payment_profiles/{id}/deposit_request | x-uber-token | amount |
| /rt/payment/payment_profiles/{id}/get_backing_instruments |||
| /rt/payment/paytm/payment_profiles/{payment_profile_uuid}/user-details |||
| /rt/communications/messages/{threadId}/{fromSequenceNumber} | x-uber-token ||
| /rt/communications/messages/trip/{tripId} | x-uber-token <br /> x-uber-uuid <br /> x-uber-client-name ||

```
/rt/communications/payload/{threadId}/{messageId}
/rt/riders/{uuid}/credit-balance
/rt/riders/{uuid}/unpaid-bills
/rt/riders/auth-alipay
/rt/riders/sign-rsa
/rt/fare/estimate
/rt/invitations
/rt/locations/locations
/rt/locations/tag/locations
/rt/locations/upfront
/rt/locations/v2/prediction/details
/rt/locations/v2/predictions
/rt/locations/v2/predictions
/rt/locations/v2/predictions
/rt/locations/v2/predictions
/rt/locations/v2/search
/rt/payment/payment_profiles/{id}/balance
/rt/payment/payment_profiles/{id}/deposit_request
/rt/inventory/shop_info?device_type=android
/rt/utunes/providers/{provider_id}
/rt/utunes/providers/{provider_id}/playlists/{playlist_id}
/rt/utunes/providers/{provider_id}/search
/rt/locations/pickups/geocode_region
/rt/locations/pickups/snap
/rt/locations/pickups/snap
/rt/locations/pickups/venue
/rt/locations/pickups/venue
/rt/config/all-experiments
/rt/config/experiments
/rt/riders/sign-rsa
/rt/referrals/campaign
/rt/referrals/get-referral-info
/rt/payment/payment_profiles/{uuid}/balance
/rt/payment/payment_profiles/{uuid}/deposit_request
/rt/payment/payment-profiles/{uuid}/airtel-money/bonus-status
/rt/riders/baidu-wallet/connect
/rt/contacts/{contactUuid}
/rt/contacts/user/{userUuid}/contacts
/rt/contacts/user/{userUuid}/contacts
/rt/contacts/v2/{contactUuid}
/rt/support/custom-nodes/appease-bad-route/{tripId}
/rt/support/custom-nodes/appease-rider-cancellation/{tripId}
/rt/users/fapiao/trips
/rt/users/fapiao/user-defaults
/rt/loyalty/user
/rt/loyalty/user/history
/rt/users/rewards
/rt/users/life/articles
/rt/users/life/articles/categories
/rt/users/life/articles/{itemUUID}
/rt/admin/users/me/test_accounts
/rt/cardoffer/offers
/rt/riders/get-earned-rides
/rt/cobrand/{clientId}
/rt/contacts/{contactUuid}
/rt/contacts/user/{userUuid}/contacts
/rt/locations/pickups/dynamic
/rt/locations/pickups/dynamic
/rt/eats/v1/get-promotion-info
/rt/family/group/{groupUuid}
/rt/family/invites
/rt/geocoding/reverse
/rt/product/hop/{vvid}/nearbyRoutes
/rt/locations/pickups/venue
/rt/locations/pool_ads
/rt/mobile/lookup-upgrade
/rt/onboarding/partner-onboarding-app/pitch-info
/rt/onboarding/partner-onboarding-app/tutorial-info
/rt/saffron/campaigns
/rt/product/city/rider-view
/rt/referrals/campaign
/rt/referrals/get-referral-info
/rt/reminders/{reminderUuid}
/rt/reminders/upcoming-for-destination-dropdown
/rt/reservation/fare-estimate
/rt/reservation/feasibility
/rt/reservation/list
/rt/riders/get-estimated-pre-trip-promotion
/rt/riders/inviter-give-get-description
/rt/riders/me/dispatch-view
/rt/riders/{riderUuid}/unpaid-bills
/rt/riders/sign-rsa
/rt/riders/unexpired-and-valid-promotions
/rt/safetynet/users/{userUuid}/contacts
/rt/trips/{tripUuid}/cancellation-info
/rt/trips/{tripUuid}/contacts
/rt/trips/{tripUuid}/route
/rt/trips/{tripUuid}/share-yo-ride
/rt/users/notification-settings
```

**POST:**

```
/rt/onboarding/documents
/rt/onboarding/dynamic-form/v2/step/{driverUUID}
/rt/onboarding/dynamic-form/v2/step/{driverUUID}
/rt/onboarding/vehicle-inspection/email/{driverUUID}
/rt/onboarding/dynamic-form/verify-phone
/rt/users/login
/rt/users/request-sms-verification
/rt/drivers/v2/{driverUUID}/vault
/rt/onboarding/send_comms
/rt/onboarding/step/{partnerUuid}
/rt/onboarding/unified-step/{partnerUuid}
/rt/onboarding/dynamic-form/signup
/rt/onboarding/dynamic-form/upgrade
/rt/payment/payment_profiles/{uuid}/reward
/rt/payment/payment_profiles/{uuid}/validation_code/validate
/rt/payment/v2/payment_profiles
/rt/payment/v2/payment_profiles
/rt/communications/message
/rt/users/request-mobile-confirmation
/rt/users/verify-password
/rt/users/passwordless-signup/add-password
/rt/invitations
/rt/users/passwordless-signup
/rt/users/reset-password
/rt/payment/payment_profiles/{id}/validation_code/send
/rt/payment/payment_profiles/{id}/validation_code/validate
/rt/payment/payment_profiles/{id}/validation_code/validate
/rt/trips/{trip_id}/anonymous-number
/rt/trips/{trip_id}/inbound-call
/rt/fare/eats_estimate
/rt/fare/eats_estimate
/rt/feedback
/rt/inventory/reminder
/rt/utunes/providers/{id}/start_trial
/rt/utunes/rider/handshake
/rt/users/two-factor-auth
/rt/rtnow/add-credentials
/rt/rtnow/check-credentials
/rt/chat/v2/new-session
/rt/invitations/{driverUUID}/contacts
/rt/invitations/{driverUUID}/contacts
/rt/invitations/{driverUUID}/nominees
/rt/referrals/bulk-invitation
/rt/referrals/create-directed-referral-code-links
/rt/referrals/create-indirect-invite
/rt/referrals/create-referral-code-links
/rt/client-promotions
/rt/payment/payment_profiles/
/rt/payment/payment_profiles/{uuid}/validation_code/send
/rt/payment/payment_profiles/{uuid}/validation_code/validate
/rt/payment/payment-profiles/{uuid}/airtel-money/deposit
/rt/payment/providers/airtel-money/account
/rt/payment/providers/airtel-money/account/link
/rt/payment/providers/airtel-money/validation-code/send
/rt/payment/providers/airtel-money/validation-code/validate
/rt/payment/payment_profiles/
/rt/payment/payment_profiles/
/rt/payment/payment_profiles/
/rt/contacts/{contactUuid}
/rt/contacts/v2/{contactUuid}
/rt/questions/get-employee-feedback
/rt/questions/record-employee-feedback
/rt/support/contacts/appease-bad-route
/rt/support/contacts/appease-rider-cancellation
/rt/support/nodes/{nodeId}/csat
/rt/users/fapiao/request
/rt/mobile/task/create
/rt/mobile/task/teams
/rt/users/rewards/{itemUUID}/action
/rt/apps/bootstrap-rider
/rt/business/redeem-employee-invite
/rt/riders/create-promotion-redemption-override
/rt/mobrec/is-eligible
/rt/mobrec/is-trip-eligible
/rt/mobrec/send-email
/rt/mobrec/update-challenge-status
/rt/riders/{riderUuid}/commute-optin-state
/rt/companies/get-company-brand
/rt/contacts/{contactUuid}/message
/rt/drivers/{driverUuid}/send-ramen-message
/rt/expensecodes/get-expense-codes-for-user
/rt/expensecodes/get-expense-codes-metadata-for-user
/rt/family/bootstrap/settings
/rt/family/group/{groupUuid}
/rt/family/group/{groupUuid}/jobs
/rt/family/group/{groupUuid}/paymentProfiles
/rt/family/invite/redeem
/rt/fare/eats_estimate
/rt/feedback/personal_transport
/rt/feedback/search-dynamic-tags
/rt/invitations/{userUuid}/contacts
/rt/invitations/{userUuid}/invites-log
/rt/invitations/{userUuid}/nominees
/rt/navigation/v2/route
/rt/notifier/device-tokens
/rt/payment/payment_profiles/{uuid}/reward
/rt/payment/v2/payment_profiles
/rt/profiles/delete-profile
/rt/profiles/get-profiles
/rt/profiles/get-profile-theme-options
/rt/profiles/onboard-user
/rt/profiles/patch-profile
/rt/profiles/request-verification
/rt/profiles/update-profile
/rt/reservation/{reservationUuid}
/rt/offers/activate-offers
/rt/offers/enroll-user
/rt/offers/get-user-offers
/rt/offers/unenroll-user
/rt/riders/me/accept-fare-split
/rt/riders/me/add-expense-info
/rt/riders/me/client-status
/rt/riders/me/decline-fare-split
/rt/riders/me/fare-estimate
/rt/riders/me/invite-fare-split
/rt/riders/me/pickup
/rt/riders/me/schedule-surge-drop
/rt/riders/me/select-payment-profile
/rt/riders/me/select-profile
/rt/riders/me/set-use-credits
/rt/riders/me/status
/rt/riders/me/uninvite-fare-split
/rt/riders/{riderUuid}/enable-emergency
/rt/riders/update-national-id
/rt/safetynet/users/{userUuid}/create-contacts
/rt/surge/input
/rt/trips/{tripUuid}/anonymous-on-demand
/rt/trips/{tripUuid}/rider-cancel
/rt/trips/{tripUuid}/rider-rate
/rt/trips/{tripUuid}/rider-set-info
/rt/trips/{tripUuid}/share-with-contacts
/rt/sharetrip/fetch
/rt/users/apply-clients-promotions
/rt/users/authenticate-third-party
/rt/users/confirm-mobile
/rt/users/login
/rt/users/picture
/rt/users/tag-user-public
/rt/users/third-party-identities
/rt/users/v2/request-mobile-confirmation
/rt/users/v2/verify-password
/rt/users/validate-promotion
```

**PUT:**

```
/rt/payment/client_bills/{bill_uuid}
/rt/payment/v2/payment_profiles/{uuid}
/rt/riders/{uuid}/confirm-mobile
/rt/riders/{uuid}/confirm-mobile
/rt/locations/tag/locations/{tag}
/rt/inventory/reminder/{uuid}
/rt/invitations/{driverUUID}/privacy
/rt/payment/client_bills/charge_synchronously/{billUuid}
/rt/payment/client_bills/charge_synchronously/{billUuid}
/rt/users/update-password
/rt/users/v3/forgot-password
/rt/family/group
/rt/family/group/{groupUuid}/members
/rt/payment/client_bills/{uuid}
/rt/payment/v2/payment_profiles/{uuid}
/rt/reservation/new
/rt/riders/me/suspend-walk-direction
/rt/riders/{riderUuid}/disable-emergency
/rt/safetynet/users/{userUuid}/delete-contacts
```

**DELETE:**

```
/rt/payment/payment_profiles/{uuid}/
/rt/locations/tag/locations/{tag}
/rt/inventory/reminder/{uuid}
/rt/invitations/{driverUUID}/contacts
/rt/payment/payment_profiles/{uuid}/
/rt/family/group/{groupUuid}
/rt/family/group/{groupUuid}/members/{memberUuid}
/rt/invitations/{userUuid}/contacts
/rt/notifier/device-tokens/{deviceToken}
/rt/payment/v2/payment_profiles/{uuid}
/rt/reservation/{reservationUuid}
/rt/users/third-party-identities/{identityType}
```
