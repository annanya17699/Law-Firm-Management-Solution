# Standard Profile Bases for Custom Profiles

## 1. System Administrator
- **Base Profile**: System Administrator
- **Rationale**: This is a standard profile and should be used as-is for system administrators.

## 2. Managing Partner Profile

- **Base Profile**: Standard User
- **Rationale**: Provides access to standard CRM objects including Cases.
- **Key Modifications**:
  - Add "Modify All Data" and "View All Data" permissions
  - Enhance permissions for all relevant standard and custom objects

## 3. Partner Profile
- **Base Profile**: Standard User
- **Rationale**: Partners need access to most standard objects and functionality.
- **Key Modifications**:
  - Add "View All Data" permission
  - Increase access levels for specific objects

## 4. Associate Attorney Profile
- **Base Profile**: Standard User
- **Rationale**: Associates need access to core CRM functionality.
- **Key Modifications**:
  - Adjust object permissions to match role requirements
  - Remove unnecessary permissions for marketing or advanced sales features

## 5. Paralegal Profile
- **Base Profile**: Standard Platform User
- **Rationale**: Paralegals need custom object access but may not need all standard CRM objects.
- **Key Modifications**:
  - Add permissions for custom objects (e.g., Legal Cases)
  - Grant limited access to standard objects like Accounts and Contacts

## 6. Operations Manager Profile
- **Base Profile**: Standard Platform User
- **Rationale**: Operations Managers need broad access but not necessarily to all sales and marketing features.
- **Key Modifications**:
  - Add "View All Data" permission
  - Grant access to reporting and dashboard management
  - Add permissions for administrative objects

## 7. Administrative Staff Profile
- **Base Profile**: Standard Platform User
- **Rationale**: Administrative staff need basic access to custom functionality and limited standard object access.
- **Key Modifications**:
  - Add permissions for relevant custom objects
  - Grant limited access to standard objects like Contacts and Calendar

## Implementation Steps:
1. Navigate to Setup > Users > Profiles
2. Find the relevant standard profile
3. Click "Clone" next to the profile name
4. Name the new profile according to your scheme (e.g., "Law Firm - Partner")
5. Modify the cloned profile permissions as needed

## Best Practices:
- Always start with the least privileged profile that meets most of the role's needs, then add permissions.
- Use Permission Sets for additional, specific permissions that only some users in a profile might need.
- Regularly review and audit custom profiles to ensure they don't accumulate unnecessary permissions over time.

## Next Steps:
1. Review these base profile recommendations and adjust if needed for your specific implementation.
2. Begin creating your custom profiles in Salesforce, starting with the clone of the recommended standard profile.
3. Document any significant deviations from these recommendations for future reference.
4. Test each profile thoroughly to ensure it provides the correct level of access for its intended role.
