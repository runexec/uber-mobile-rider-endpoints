# uber-mobile-rider-endpoints
Unofficial Documentation of Uber Endpoints (Rider)

Work in progress

**Possible Hosts:**


```
https://cn-dc1.uber.com 
https://cn.uber.com
```

| Req | Path | Required Headers | Required Params |
|-----|------|------------------|------------------|
| GET | /rt/onboarding/dynamic-form/step/{driverUUID} | x-uber-token ||
| GET | /rt/onboarding/signup | x-uber-device-language ||
| GET | /rt/drivers/{driverUUID}/vault | x-uber-token ||
| GET | /rt/onboarding/step/{partnerUuid} | x-uber-onboarding-variant <br /> x-uber-token ||
| GET | /rt/onboarding/unified-step/{partnerUuid} | x-uber-onboarding-variant <br /> x-uber-token ||
| GET | /rt/onboarding/dynamic-form/signup |||
| GET | /rt/onboarding/dynamic-form/upgrade |||
| GET | /rt/payment/payment_profiles/{id}/balance | x-uber-token ||
| GET | /rt/payment/v2/payment_profiles | x-uber-token ||
| GET | /rt/payment/payment_profiles/{id}/deposit_request | x-uber-token | amount |
| GET | /rt/payment/payment_profiles/{id}/get_backing_instruments |||
| GET | /rt/payment/paytm/payment_profiles/{payment_profile_uuid}/user-details |||
| GET | /rt/communications/messages/{threadId}/{fromSequenceNumber} | x-uber-token ||
| GET | /rt/communications/messages/trip/{tripId} | x-uber-token <br /> x-uber-uuid <br /> x-uber-client-name ||
| GET | /rt/communications/payload/{threadId}/{messageId} | x-uber-token ||
| GET | /rt/riders/{uuid}/credit-balance | x-uber-token ||
| GET | /rt/riders/{uuid}/unpaid-bills  | x-uber-token ||
| GET | /rt/riders/auth-alipay |||
| GET | /rt/riders/sign-rsa || input |
| GET | /rt/fare/estimate || origin_lat <br /> origin_lng <br /> vehicle_view_ids <br /> destination_lat <br /> destination_lng |
| GET | /rt/invitations  | x-uber-token ||
| GET | /rt/locations/locations |||
| GET | /rt/locations/tag/locations |||
| GET | /rt/locations/upfront |||
| GET | /rt/locations/v2/prediction/details |||
| GET | /rt/locations/v2/predictions |||
| GET | /rt/locations/v2/search |||
| GET | /rt/payment/payment_profiles/{id}/balance | x-uber-token ||
| GET | /rt/inventory/shop_info?device_type=android |||
| GET | /rt/utunes/providers/{provider_id} | x-uber-token ||
| GET | /rt/utunes/providers/{provider_id}/playlists/{playlist_id} | x-uber-token ||
| GET | /rt/utunes/providers/{provider_id}/search | x-uber-token | query |
| GET | /rt/locations/pickups/geocode_region |||
| GET | /rt/locations/pickups/snap |||
| GET | /rt/locations/pickups/venue |||
| GET | /rt/config/all-experiments | x-uber-token ||
| GET | /rt/config/experiments |||
| GET | /rt/riders/sign-rsa || input |
| GET | /rt/referrals/campaign | x-uber-token ||
| GET | /rt/referrals/get-referral-info | x-uber-token ||
| GET | /rt/payment/payment_profiles/{uuid}/balance | x-uber-token ||
| GET | /rt/payment/payment_profiles/{uuid}/deposit_request | x-uber-token | amount |
| GET | /rt/payment/payment-profiles/{uuid}/airtel-money/bonus-status |||
| GET | /rt/riders/baidu-wallet/connect | x-uber-token | pageUrl |
| GET | /rt/contacts/{contactUuid} | x-uber-token ||
| GET | /rt/contacts/user/{userUuid}/contacts | x-uber-token ||
| GET | /rt/contacts/v2/{contactUuid} | x-uber-token ||
| GET | /rt/support/custom-nodes/appease-bad-route/{tripId} | x-uber-token ||
| GET | /rt/support/custom-nodes/appease-rider-cancellation/{tripId} | x-uber-token ||
| GET | /rt/users/fapiao/trips | x-uber-token | tripType <br /> offset |
| GET | /rt/users/fapiao/user-defaults | x-uber-token ||
| GET | /rt/loyalty/user | x-uber-token <br /> x-uber-uuid <br /> x-uber-device <br /> x-uber-device-language <br /> x-uber-client-name <br /> x-uber-client-version <br /> x-uber-device-location-latitude <br /> x-uber-device-location-longitude | |
| GET | /rt/loyalty/user/history | x-uber-token <br /> x-uber-uuid <br /> x-uber-device <br /> x-uber-device-language <br /> x-uber-client-name <br /> x-uber-client-version <br /> x-uber-device-location-latitude <br /> x-uber-device-location-longitude||
| GET | /rt/users/rewards | x-uber-token | offset <br /> count <br /> type |
| GET | /rt/users/life/articles | x-uber-uuid <br /> x-uber-token <br /> x-uber-device <br /> x-uber-device-language <br /> x-uber-client-name <br /> x-uber-client-version <br /> x-uber-device-location-latitude <br /> x-uber-device-location-longitude | category |
| GET | /rt/users/life/articles/categories | x-uber-uuid <br /> x-uber-token <br /> x-uber-device <br /> x-uber-device-language <br /> x-uber-client-name <br /> x-uber-client-version <br /> x-uber-device-location-latitude <br /> x-uber-device-location-longitude ||
| GET | /rt/users/life/articles/{itemUUID} | x-uber-uuid <br /> x-uber-token <br /> x-uber-device <br /> x-uber-device-language <br /> x-uber-client-name <br /> x-uber-client-version <br /> x-uber-device-location-latitude <br /> x-uber-device-location-longitude | provider <br /> category |
| GET | /rt/admin/users/me/test_accounts | x-uber-token | role |
| GET | /rt/cardoffer/offers | x-uber-token ||
| GET | /rt/riders/get-earned-rides | x-uber-token ||
| GET | /rt/cobrand/{clientId} | x-uber-token ||
| GET | /rt/contacts/{contactUuid} | x-uber-token ||
| GET | /rt/contacts/user/{userUuid}/contacts | x-uber-token || 
| GET | /rt/locations/pickups/dynamic |||
| GET | /rt/eats/v1/get-promotion-info |||
| GET | /rt/family/group/{groupUuid} |||
| GET | /rt/family/invites |||
| GET | /rt/geocoding/reverse | x-uber-token | latitude <br /> longitude <br /> language |
| GET | /rt/product/hop/{vvid}/nearbyRoutes | x-uber-token ||
| GET | /rt/locations/pickups/venue |||
| GET | /rt/locations/pool_ads |||
| GET | /rt/mobile/lookup-upgrade | x-uber-token | appName |
| GET | /rt/onboarding/partner-onboarding-app/pitch-info |||
| GET | /rt/onboarding/partner-onboarding-app/tutorial-info |||
| GET | /rt/saffron/campaigns |||
| GET | /rt/product/city/rider-view |||
| GET | /rt/referrals/campaign | x-uber-token ||
| GET | /rt/referrals/get-referral-info | x-uber-token ||
| GET | /rt/reminders/{reminderUuid} | x-uber-token | clientId |
| GET | /rt/reminders/upcoming-for-destination-dropdown | x-uber-token | userUuid |
| GET | /rt/reservation/fare-estimate | x-uber-token <br /> | originLat <br /> originLng <br /> destinationLat <br /> destinationLng <br /> vehicleViewId |
| GET | /rt/reservation/feasibility | | originLat <br /> originLng |
| GET | /rt/reservation/list | x-uber-token ||
| GET | /rt/riders/get-estimated-pre-trip-promotion || originLat <br /> originLng <br /> vehicleViewIds |
| GET | /rt/riders/inviter-give-get-description | x-uber-token ||
| GET | /rt/riders/me/dispatch-view | x-uber-token ||
| GET | /rt/riders/{riderUuid}/unpaid-bills | x-uber-token ||
| GET | /rt/riders/sign-rsa || input |
| GET | /rt/riders/unexpired-and-valid-promotions |||
| GET | /rt/safetynet/users/{userUuid}/contacts | x-uber-token ||
| GET | /rt/trips/{tripUuid}/cancellation-info |||
| GET | /rt/trips/{tripUuid}/contacts | x-uber-token ||
| GET | /rt/trips/{tripUuid}/route | x-uber-token ||
| GET | /rt/trips/{tripUuid}/share-yo-ride | x-uber-token ||
| GET | /rt/users/notification-settings | x-uber-token <br /> x-uber-uuid <br /> x-uber-device-language ||

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
