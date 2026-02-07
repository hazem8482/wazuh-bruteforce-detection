Wazuh – Windows Brute Force (4625)

Detect brute-force login attempts on Windows using Wazuh.

Event ID: 4625 (Failed logon)

Base rule: 60122

Custom rule: 100501 (Level 12)

<rule id="100501" level="12">
  <if_matched_sid>60122</if_matched_sid>
  <description>Possible Windows brute-force detected</description>
</rule>


Attack test: multiple failed net use logins
Result: alert triggered in Wazuh
