# Big list of tools, exploits, whatever I felt needed to be here and how to use them
This is a modified list of the pentest-standard.org technical guidelines. The site misses a few things involving social engineering, physec, buffer overflows and some others. I've (hopefully) compressed the table of contents a bit and added to the document.


##### Table of Contents  

1 Tools_Required <details><summary>Show</summary><p> 
   - 1.1 Operating_Systems
      + 1.1.1 MacOS_X
      + 1.1.2 VMware_Workstation
         * 1.1.2.1 Linux
         * 1.1.2.2 Windows_XP/7
    - 1.2 Radio_Frequency_Tools 
      + 1.2.1 Frequency_Counter
      + 1.2.2 Frequency_Scanner
      + 1.2.3 Spectrum_Analyzer
      + 1.2.4 802.11_USB_adapter
      + 1.2.5 External_Antennas
      + 1.2.6 USB_GPS
    - 1.3 Software  </p></details>
   
   
   
   2 Intelligence Gathering <details><summary>Show</summary><p>
   
        2.1 OSINT 
            2.1.1 Corporate
            2.1.2 Physical
                2.1.2.1 Locations
                2.1.2.2 Shared/Individual
                2.1.2.3 Owner
                    2.1.2.3.1 Land/tax_records
   
            2.1.3 Datacenter_Locations
                2.1.3.1 Time_zones
                2.1.3.2 Offsite_gathering
                2.1.3.3 Product/Services
                2.1.3.4 Company_Dates
                2.1.3.5 Position_identification
                2.1.3.6 Organizational_Chart
                2.1.3.7 Corporate_Communications
                    2.1.3.7.1 Marketing
                    2.1.3.7.2 Lawsuits
                    2.1.3.7.3 Transactions
                2.1.3.8 Job_openings
            2.1.4 Relationships
                2.1.4.1 Charity_Affiliations
                2.1.4.2 Network_Providers
                2.1.4.3 Business_Partners
                2.1.4.4 Competitors
        2.2 Individuals
            2.2.1 Social_Networking_Profile
            2.2.2 Social_Networking_Websites
            2.2.3 Cree.py
        2.3 Internet_Footprint
            2.3.1 Email_addresses
                2.3.1.1 Maltego
                2.3.1.2 TheHarvester
                2.3.1.3 NetGlub
            2.3.2 Usernames/Handles
            2.3.3 Social_Networks
                2.3.3.1 Newsgroups
                2.3.3.2 Mailing_Lists
                2.3.3.3 Chat_rooms
                2.3.3.4 Forums_Search
            2.3.4 Personal_Domain_Names
            2.3.5 Personal_Activities
                2.3.5.1 Audio
                2.3.5.2 Video
            2.3.6 Archived_Information
            2.3.7 Electronic_Data
                2.3.7.1 Document_leakage
                2.3.7.2 Metadata_leakage
                    2.3.7.2.1 FOCA_(Windows)
                    2.3.7.2.2 Foundstone_SiteDigger_(Windows)
                    2.3.7.2.3 Metagoofil_(Linux/Windows)
                    2.3.7.2.4 Exif Reader_(Windows)
                    2.3.7.2.5 ExifTool_(Windows/ OS X)
                    2.3.7.2.6 Image_Search
        2.4 Covert_gathering
            2.4.1 On-location_gathering
                2.4.1.1 Adjacent_Facilities
                2.4.1.2 Physical_security_inspections
                    2.4.1.2.1 Security_guards
                    2.4.1.2.2 Badge_Usage
                    2.4.1.2.3 Locking_devices
                    2.4.1.2.4 Intrusion_detection_systems_(IDS)/Alarms
                    2.4.1.2.5 Security_lighting
                    2.4.1.2.6 Surveillance_/CCTV_systems
                    2.4.1.2.7 Access_control_devices
                    2.4.1.2.8 Environmental_Design
                2.4.1.3 Employee_Behavior
                2.4.1.4 Dumpster_diving
                2.4.1.5 RF_/Wireless_Frequency_scanning
            2.4.2 Frequency_Usage
            2.4.3 Equipment_Identification
                2.4.3.1 Airmon-ng
                2.4.3.2 Airodump-ng
                2.4.3.3 Kismet-Newcore
                2.4.3.4 inSSIDer
        2.5 External_Footprinting
            2.5.1 Identifying_IP_Ranges
                2.5.1.1 WHOIS_lookup
                2.5.1.2 BGP_looking_glasses
            2.5.2 Active_Reconnaissance
            2.5.3 Passive_Reconnaissance
            2.5.4 Active_Footprinting
                2.5.4.1 Zone_Transfers
                    2.5.4.1.1 Host
                    2.5.4.1.2 Dig
                2.5.4.2 Reverse_DNS
                2.5.4.3 DNS_Bruting
                    2.5.4.3.1 Fierce2_(Linux)
                    2.5.4.3.2 DNSEnum_(Linux)
                    2.5.4.3.3 Dnsdict6_(Linux)
                2.5.4.4 Port_Scanning
                    2.5.4.4.1 Nmap_(Windows/Linux)
                2.5.4.5 SNMP_Sweeps
                    2.5.4.5.1 SNMPEnum_(Linux)
                2.5.4.6 SMTP_Bounce_Back
                2.5.4.7 Banner_Grabbing
                    2.5.4.7.1 HTTP
        2.6 Internal_Footprinting
            2.6.1 Active_Footprinting
                2.6.1.1 Ping_Sweeps
                    2.6.1.1.1 Nmap_(Windows/Linux)
                    2.6.1.1.2 Alive6_(Linux)
                2.6.1.2 Port_Scanning
                    2.6.1.2.1 Nmap_(Windows/Linux)
                2.6.1.3 SNMP_Sweeps
                    2.6.1.3.1 SNMPEnum_(Linux)
                2.6.1.4 Metasploit
                2.6.1.5 Zone_Transfers
                    2.6.1.5.1 Host
                    2.6.1.5.2 Dig
                2.6.1.6 SMTP_Bounce_Back
                2.6.1.7 Reverse_DNS
                2.6.1.8 Banner_Grabbing
                    2.6.1.8.1 HTTP
                    2.6.1.8.2 httprint
                2.6.1.9 VoIP_mapping
                    2.6.1.9.1 Extensions
                    2.6.1.9.2 Svwar
                    2.6.1.9.3 enumIAX
                2.6.1.10 Passive_Reconnaissance
                    2.6.1.10.1 Packet_Sniffing
                    
  </p></details>
                     
                     
   3 Vulnerability_Analysis <details><summary>Show</summary><p> 
        3.1 Vulnerability Testing
            3.1.1 Active
            3.1.2 Automated_Tools
                3.1.2.1 Network/General_Vulnerability_Scanners
                3.1.2.2 Open Vulnerability_Assessment_System_(OpenVAS)(Linux)
                3.1.2.3 Nessus_(Windows/Linux)
                3.1.2.4 NeXpose
                3.1.2.5 eEYE_Retina
                3.1.2.6 Qualys
                3.1.2.7 Core_IMPACT
                    3.1.2.7.1 Core_IMPACT_Web
                    3.1.2.7.2 Core_IMPACT_WiFi
                    3.1.2.7.3 Core_IMPACT_Client Side
                    3.1.2.7.4 Core_Web
                    3.1.2.7.5 coreWEBcrawl
                    3.1.2.7.6 Core_Onestep_Web_RPTs
                    3.1.2.7.7 Core_WiFi
                3.1.2.8 SAINT
                    3.1.2.8.1 SAINTscanner
                    3.1.2.8.2 SAINTexploit
                    3.1.2.8.3 SAINTwriter
            3.1.3 Web_Application_Scanners
                3.1.3.1 General_Web_Application_Scanners
                    3.1.3.1.1 WebInspect_(Windows)
                    3.1.3.1.2 IBM_AppScan
                    3.1.3.1.3 Web_Directory_Listing/Bruteforcing
                    3.1.3.1.4 Webserver_Version/Vulnerability_Identification
                3.1.3.2 NetSparker_(Windows)
                3.1.3.3 Specialized_Vulnerability Scanners
                    3.1.3.3.1 Virtual_Private_Networking_(VPN)
                    3.1.3.3.2 IPv6
                    3.1.3.3.3 War_Dialing
            3.1.4 Passive_Testing
                3.1.4.1 Automated_Tools
                    3.1.4.1.1 Traffic_Monitoring
                3.1.4.2 Wireshark
                3.1.4.3 Tcpdump
                3.1.4.4 Metasploit_Scanners
                    3.1.4.4.1 Metasploit_Unleashed
        3.2 Vulnerability_Validation
            3.2.1 Public_Research
                3.2.1.1 Common/default_passwords
            3.2.2 Establish_target_list
                3.2.2.1 Mapping_Versions
                3.2.2.2 Identifying_Patch_Levels
                3.2.2.3 Looking_for_Weak_Web_Applications
                3.2.2.4 Identify_Weak_Ports_and_Services
                3.2.2.5 Identify_Lockout_threshold
        3.3 Attack_Avenues
            3.3.1 Creation_of_Attack_Trees
            3.3.2 Identify_protection_mechanisms
                3.3.2.1 Network_protections
                    3.3.2.1.1 "Simple"Packet_Filters
                    3.3.2.1.2 Traffic_shaping_devices
                    3.3.2.1.3 Data_Loss_Prevention_(DLP)systems
                3.3.2.2 Host_based_protections
                    3.3.2.2.1 Stack/heap_protections
                    3.3.2.2.2 Whitelisting
                    3.3.2.2.3 AV/Filtering/Behavioral_Analysis
                3.3.2.3 Application_level_protections
   
   </p></details>
   
   
   4 Exploitation <details><summary>Show</summary><p> 
        4.1 Precision_strike
            4.1.1 Countermeasure_Bypass
                4.1.1.1 AV
                4.1.1.2 Human
                4.1.1.3 HIPS
                4.1.1.4 DEP
                4.1.1.5 ASLR
                4.1.1.6 VA _+_NX_(Linux)
                4.1.1.7 w^x_(OpenBSD)
                4.1.1.8 WAF
                4.1.1.9 Stack_Canaries
                    4.1.1.9.1 Microsoft_Windows
                    4.1.1.9.2 Linux
                    4.1.1.9.3 MAC_OS
        4.2 Customized_Exploitation
            4.2.1 Fuzzing
            4.2.2 Dumb_Fuzzing
            4.2.3 Intelligent_Fuzzing
            4.2.4 Sniffing
                4.2.4.1 Wireshark
                4.2.4.2 Tcpdump
            4.2.5 Brute-Force
                4.2.5.1 Brutus_(Windows)
                4.2.5.2 Web Brute_(Windows)
                4.2.5.3 THC-Hydra/XHydra
                4.2.5.4 Medusa
                4.2.5.5 Ncrack
            4.2.6 Routing_protocols
            4.2.7 Cisco_Discovery_Protocol(CDP)
            4.2.8 Hot_Standby_Router_Protocol(HSRP)
            4.2.9 Virtual_Switch_Redundancy_Protocol(VSRP)
            4.2.10 Dynamic_Trunking_Protocol(DTP)
            4.2.11 Spanning_Tree_Protocol(STP)
            4.2.12 Open_Shortest_Path First(OSPF)
            4.2.13 RIP
            4.2.14 VLAN_Hopping
            4.2.15 VLAN_Trunking_Protocol(VTP)
        4.3 RF_Access
            4.3.1 Unencrypted_Wireless_LAN
                4.3.1.1 Iwconfig_(Linux)
                4.3.1.2 Windows_(XP/7)
            4.3.2 Attacking_the_Access_Point
                4.3.2.1 Denial_of_Service(DoS)
            4.3.3 Cracking_Passwords
                4.3.3.1 WPA-PSK/WPA2-PSK
                4.3.3.2 WPA/WPA2-Enterprise
            4.3.4 Attacks
                4.3.4.1 LEAP
                    4.3.4.1.1 Asleap
                4.3.4.2 802.1X
                    4.3.4.2.1 Key_Distribution_Attack
                    4.3.4.2.2 RADIUS_Impersonation_Attack
                4.3.4.3 PEAP
                    4.3.4.3.1 RADIUS_Impersonation_Attack
                    4.3.4.3.2 Authentication_Attack
                4.3.4.4 EAP-Fast
                4.3.4.5 WEP/WPA/WPA2
                4.3.4.6 Aircrack-ng
        4.4 Attacking_the_User
            4.4.1 Karmetasploit_Attacks
            4.4.2 DNS_Requests
            4.4.3 Bluetooth
            4.4.4 Personalized_Rogue_AP
            4.4.5 Web
                4.4.5.1 SQL_Injection_(SQLi)
                4.4.5.2 XSS
                4.4.5.3 CSRF
            4.4.6 Ad-Hoc_Networks
            4.4.7 Detection_bypass
            4.4.8 Resistance_of_Controls_to_attacks
            4.4.9 Type_of_Attack
            4.4.10 The_Social-Engineer_Toolkit
        4.5 VPN_detection
        4.6 Route_detection,including_static_routes
            4.6.1 Network_Protocols_in_use
            4.6.2 Proxies_in_use
            4.6.3 Network_layout
            4.6.4 High_value/profile_targets
        4.7 Pillaging
            4.7.1 Video_Cameras
            4.7.2 Data_Exfiltration
            4.7.3 Locating_Shares
            4.7.4 Audio_Capture
            4.7.5 High_Value_Files
            4.7.6 Database_Enumeration
            4.7.7 Wifi
            4.7.8 Source_Code_Repos
            4.7.9 Git
            4.7.10 Identify_custom_apps
            4.7.11 Backups
        4.8 Business_impact_attacks
        4.9 Further_penetration_into_infrastructure
            4.9.1 Pivoting_inside
                4.9.1.1 History/Logs
            4.9.2 Cleanup
        4.10 Persistence
        </p></details>
        
        
        
  5 Post Exploitation <details><summary>Show</summary><p> 
        5.1 Windows_Post_Exploitation
            5.1.1 Blind_Files
            5.1.2 Non_Interactive_Command_Execution
            5.1.3 System
            5.1.4 Networking_(ipconfig,netstat,net)
            5.1.5 Configs
            5.1.6 Finding_Important_Files
            5.1.7 Files_To_Pull_(if possible)
            5.1.8 Remote_System_Access
            5.1.9 Auto-Start_Directories
            5.1.10 Binary_Planting
            5.1.11 Deleting_Logs
            5.1.12 Uninstalling_Software_“AntiVirus”_(Non_interactive)
            5.1.13 Other
                5.1.13.1 Operating_Specific
                    5.1.13.1.1 Win2k3
                    5.1.13.1.2 Vista/7
                    5.1.13.1.3 Vista_SP1/7/2008/2008R2_(x86_&\_x64)
            5.1.14 Invasive_or_Altering_Commands
            5.1.15 Support_Tools_Binaries_/Links_/Usage
                5.1.15.1 Various_tools
        5.2 Obtaining_Password_Hashes_in_Windows
            5.2.1 LSASS Injection
                5.2.1.1 Pwdump6_and_Fgdump
                5.2.1.2 Hashdump_in_Meterpreter
            5.2.2 Extracting Passwords_from_Registry
                5.2.2.1 Copy_from_the_Registry
                5.2.2.2 Extracting_the_Hashes
            5.2.3 Extracting_Passwords_from_Registry_using_Meterpreter
        </p></details>
            
            
   6 Reporting <details><summary>Show</summary><p> 
        6.1 Executive-Level_Reporting
        6.2 Technical_Reporting
        6.3 Quantifying_the_risk
        6.4 Deliverable
        </p></details>
        
   7 Custom_tools_developed
    
   8 Appendix_A-Creating_OpenVAS_"Only_Safe_Checks"Policy <details><summary>Show</summary><p> 
        8.1 General
        8.2 Plugins
        8.3 Credentials
        8.4 Target_Selection
        8.5 Access_Rules
        8.6 Preferences
        8.7 Knowledge_Base
  </p></details>
  
  9 Appendix_B-Creating_the_"Only_Safe_Checks"\_Policy <details><summary>Show</summary><p> 
        9.1 General
        9.2 Credentials
        9.3 Plugins
        9.4 Preferences
        </p></details>
    
   10 Appendix_C-Creating_the_"Only_Safe_Checks_(Web)"\_Policy <details><summary>Show</summary><p> 
        10.1 General
        10.2 Credentials
        10.3 Plugins
        10.4 Preferences
    </p></details>
 
 11 Appendix_D-Creating_the_"Validation_Scan"\_Policy <details><summary>Show</summary><p> 
        11.1 General
        11.2 Credentials
        11.3 Plugins
        11.4 Preferences
        </p></details>
 
 12 Appendix_E-NeXpose_Default_Templates <details><summary>Show</summary><p> 
        12.1 Denial_of_service
        12.2 Discovery_scan
        12.3 Discovery_scan_(aggressive)
        12.4 Exhaustive
        12.5 Full_audit
        12.6 HIPAA_compliance
        12.7 Internet_DMZ_audit
        12.8 Linux_RPMs
        12.9 Microsoft_hotfix
        12.10 Payment_Card_Industry_(PCI)audit
        12.11 Penetration_test
        12.12 Penetration_test
        12.13 Safe_network_audit
        12.14 Sarbanes-Oxley_(SOX)compliance
        12.15 SCADA_audit
        12.16 Web_audit
        </p></details>


---

Ref:http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines

