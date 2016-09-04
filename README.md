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
| POST | /rt/apps/bootstrap-rider | x-uber-token ||
| POST | /rt/business/redeem-employee-invite || request |
| POST | /rt/chat/v2/new-session | x-uber-token ||
| POST | /rt/client-promotions |||
| POST | /rt/communications/message | x-uber-token | senderId <br /> messageType <br /> clientMesssageId <br /> payload |
| POST | /rt/companies/get-company-brand | x-uber-token | request |
| POST | /rt/contacts/{contactUuid} | x-uber-token | requesterId |
| POST | /rt/contacts/{contactUuid}/message |||
| POST | /rt/contacts/v2/{contactUuid} || contactId <br /> requesterId |
| POST | /rt/drivers/{driverUuid}/send-ramen-message | x-uber-token | msg <br /> msgType |
| POST | /rt/drivers/v2/{driverUUID}/vault | x-uber-token | vault <br /> infoType|
| POST | /rt/expensecodes/get-expense-codes-for-user | x-uber-token | request |
| POST | /rt/expensecodes/get-expense-codes-metadata-for-user | x-uber-token | request |
| POST | /rt/family/bootstrap/settings || body.request |
| POST | /rt/family/group/{groupUuid} | x-uber-token ||
| POST | /rt/family/group/{groupUuid}/jobs | x-uber-token | jobUUID <br /> dc|
| POST | /rt/family/group/{groupUuid}/paymentProfiles | x-uber-token | cardNumber <br /> cardCode <br /> cardExpirationMonth <br /> cardExpirationYear <br /> billingZip <br /> paymentProfileUUID |
| POST | /rt/family/invite/redeem | x-uber-token | request |
| POST | /rt/fare/eats_estimate | x-uber-token | items <br /> vehicleViewId <br /> items <br /> vehicle_view_id|
| POST | /rt/feedback | x-uber-token | feedback |
| POST | /rt/feedback/personal_transport | x-uber-token | feedback |
| POST | /rt/feedback/search-dynamic-tags | x-uber-token | options |
| POST | /rt/inventory/reminder | x-uber-token | itemId <br /> timestamp |
| POST | /rt/invitations | x-uber-token | invitees |
| POST | /rt/invitations/{driverUUID}/nominees | x-uber-token ||
| POST | /rt/invitations/{userUuid}/contacts | x-uber-token ||
| POST | /rt/invitations/{userUuid}/invites-log | x-uber-token ||
| POST | /rt/invitations/{userUuid}/nominees | x-uber-token ||
| POST | /rt/mobile/task/create | x-uber-token | task |
| POST | /rt/mobile/task/teams | x-uber-token | clientIdentifier |
| POST | /rt/mobrec/is-eligible | x-uber-token ||
| POST | /rt/mobrec/is-trip-eligible | x-uber-token | jobUUID |
| POST | /rt/mobrec/send-email | x-uber-token | challengeId <br /> status |
| POST | /rt/mobrec/update-challenge-status | x-uber-token | challengeId <br /> status |
| POST | /rt/navigation/v2/route | x-uber-token | origin <br /> destination |
| POST | /rt/notifier/device-tokens |||
| POST | /rt/offers/activate-offers | x-uber-token | offerUuids <br /> impressionUuid |
| POST | /rt/offers/enroll-user | x-uber-token | termsVersion <br /> impressionUuid |
| POST | /rt/offers/get-user-offers | x-uber-token ||
| POST | /rt/offers/unenroll-user | x-uber-token | impressionUuid |
| POST | /rt/onboarding/documents | x-uber-token ||
| POST | /rt/onboarding/dynamic-form/signup || flow_type_city_id <br /> phone <br /> password |
| POST | /rt/onboarding/dynamic-form/upgrade || client_uuid <br /> flow_type_city_id|
| POST | /rt/onboarding/dynamic-form/verify-phone || phone_number <br /> sms_token |
| POST | /rt/onboarding/send_comms | x-uber-token | type <br /> partnerUuid|
| POST | /rt/onboarding/step/{partnerUuid} | x-uber-onboarding-variant <br /> x-uber-token | stepId |
| POST | /rt/onboarding/unified-step/{partnerUuid} | x-uber-onboarding-variant <br /> x-uber-token | stepId |
| POST | /rt/onboarding/vehicle-inspection/email/{driverUUID} | x-uber-token ||
| POST | /rt/payment/payment_profiles/ | x-uber-token | cardNumber <br /> cardCode <br /> cardExpirationMonth <br /> cardExpirationYear <br /> billingZip <br /> billingCountryIso2 <br /> tokenData <br /> tokenType <br /> token_type |
| POST | /rt/payment/payment_profiles/{id}/validation_code/send |||
| POST | /rt/payment/payment-profiles/{uuid}/airtel-money/deposit |||
| POST | /rt/payment/payment_profiles/{uuid}/reward |||
| POST | /rt/payment/payment_profiles/{uuid}/reward |||
| POST | /rt/payment/payment_profiles/{uuid}/validation_code/send |||
| POST | /rt/payment/payment_profiles/{uuid}/validation_code/validate |||
| POST | /rt/payment/payment_profiles/{uuid}/validation_code/validate |||
| POST | /rt/payment/providers/airtel-money/account |||
| POST | /rt/payment/providers/airtel-money/account/link |||
| POST | /rt/payment/providers/airtel-money/validation-code/send |||
| POST | /rt/payment/providers/airtel-money/validation-code/validate |||
| POST | /rt/payment/v2/payment_profiles |||
| POST | /rt/profiles/delete-profile |||
| POST | /rt/profiles/get-profiles |||
| POST | /rt/profiles/get-profile-theme-options |||
| POST | /rt/profiles/onboard-user |||
| POST | /rt/profiles/patch-profile |||
| POST | /rt/profiles/request-verification |||
| POST | /rt/profiles/update-profile |||
| POST | /rt/questions/get-employee-feedback |||
| POST | /rt/questions/record-employee-feedback |||
| POST | /rt/referrals/bulk-invitation |||
| POST | /rt/referrals/create-directed-referral-code-links |||
| POST | /rt/referrals/create-indirect-invite |||
| POST | /rt/referrals/create-referral-code-links |||
| POST | /rt/reservation/{reservationUuid} |||
| POST | /rt/riders/create-promotion-redemption-override |||
| POST | /rt/riders/me/accept-fare-split |||
| POST | /rt/riders/me/add-expense-info |||
| POST | /rt/riders/me/client-status |||
| POST | /rt/riders/me/decline-fare-split |||
| POST | /rt/riders/me/fare-estimate |||
| POST | /rt/riders/me/invite-fare-split |||
| POST | /rt/riders/me/pickup |||
| POST | /rt/riders/me/schedule-surge-drop |||
| POST | /rt/riders/me/select-payment-profile |||
| POST | /rt/riders/me/select-profile |||
| POST | /rt/riders/me/set-use-credits |||
| POST | /rt/riders/me/status |||
| POST | /rt/riders/me/uninvite-fare-split |||
| POST | /rt/riders/{riderUuid}/commute-optin-state |||
| POST | /rt/riders/{riderUuid}/enable-emergency |||
| POST | /rt/riders/update-national-id |||
| POST | /rt/rtnow/add-credentials |||
| POST | /rt/rtnow/check-credentials |||
| POST | /rt/safetynet/users/{userUuid}/create-contacts |||
| POST | /rt/sharetrip/fetch |||
| POST | /rt/support/contacts/appease-bad-route |||
| POST | /rt/support/contacts/appease-rider-cancellation |||
| POST | /rt/support/nodes/{nodeId}/csat |||
| POST | /rt/surge/input |||
| POST | /rt/trips/{trip_id}/anonymous-number |||
| POST | /rt/trips/{trip_id}/inbound-call |||
| POST | /rt/trips/{tripUuid}/anonymous-on-demand |||
| POST | /rt/trips/{tripUuid}/rider-cancel |||
| POST | /rt/trips/{tripUuid}/rider-rate |||
| POST | /rt/trips/{tripUuid}/rider-set-info |||
| POST | /rt/trips/{tripUuid}/share-with-contacts |||
| POST | /rt/users/apply-clients-promotions |||
| POST | /rt/users/authenticate-third-party |||
| POST | /rt/users/confirm-mobile |||
| POST | /rt/users/fapiao/request |||
| POST | /rt/users/login |||
| POST | /rt/users/login |||
| POST | /rt/users/passwordless-signup |||
| POST | /rt/users/passwordless-signup/add-password |||
| POST | /rt/users/picture |||
| POST | /rt/users/request-mobile-confirmation |||
| POST | /rt/users/request-sms-verification |||
| POST | /rt/users/reset-password |||
| POST | /rt/users/rewards/{itemUUID}/action |||
| POST | /rt/users/tag-user-public |||
| POST | /rt/users/third-party-identities |||
| POST | /rt/users/two-factor-auth |||
| POST | /rt/users/v2/request-mobile-confirmation |||
| POST | /rt/users/v2/verify-password |||
| POST | /rt/users/validate-promotion |||
| POST | /rt/users/verify-password |||
| POST | /rt/utunes/providers/{id}/start_trial |||
| POST | /rt/utunes/rider/handshake |||



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
