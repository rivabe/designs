################################################################################
#                                                                                                                                                            #
# Copyright (c) 2017 Cisco Systems                                                                                                      #
# All Rights Reserved.                                                                                                                            #
#                                                                                                                                                            #
#    Licensed under the Apache License, Version 2.0 (the "License"); you may                                       #
#    not use this file except in compliance with the License. You may obtain                                        #
#    a copy of the License at                                                                                                                   #
#                                                                                                                                                            #
#         http://www.apache.org/licenses/LICENSE-2.0                                                                          #
#                                                                                                                                                            #
#    Unless required by applicable law or agreed to in writing, software                                                #
#    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT                                    #
#    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the                            #
#    License for the specific language governing permissions and limitations                                      #
#    under the License.                                                                                                                           #
#                                                                                                                                                            #
################################################################################

Cisco ASA failover pair & FTD cluster NGIPS FPR4150s with Nexus5548 switches in vPC
========================================================
Posted configuration files showcase how to use FPR4100 appliances and Nexus5000 switches,
and build a resilient+ NGFW design with ASA Failover and a cluster of FTD inline-IPS appliances.
Failover link between ASAs is crossconnected with a cable between Eth1/8 ports. FTD apps on
FPR4150s are in a cluster running one inline set with two port pairs of port-channels.  Two
port-channels, ASA primary and secondary vPCs are being paired with their switch side via FTD
cluster.  To help with review of this setup, number of videos will be created on YouTube.

Here are the configurations included:

Two Nexus5000 switches in vPC (virtual port-channels match up to primary and secondary ASAs)
-----------------------------------------------------------------------------------
nexus5548-sw1.cfg
nexus5548-sw2.cfg

Two Firepower4100 appliances in ASA failover - Multiple contexts, all in routed firewall mode
-------------------------------------------------------------------------
fpr4150-asa-primary.cfg
fpr4150-asa-secondary.cfg

Cisco Firepower NGFW - ASA App Playlist:
https://www.youtube.com/playlist?list=PL_VvDNvGnyZ3JUoG8D4NBY-cTbiISb8Cc


Two Firepower4150 appliances running in FTD cluster - performing inline-IPS 
------------------------------------------------------------------
ftd_cluster_ngips_config.pdf.

FTD devices are managed from FMC, and those configurations are shown in the GUI.

Cisco Firepower NGFW – ASA and FTD App Playlists:
Cisco Firepower NGFW – FTD App Playlist: http://cs.co/asa-on-firepower
Cisco Firepower NGFW - ASA App Playlist: http://cs.co/ftd-on-firepower

FPR4100 FTD App Cluster NGIPS with ASA App Failover (1) Overview: https://youtu.be/-2AQt4ZxwmU

FPR4100  FTD Cluster NGIPS with ASA HA (2) Data Link Resiliency: https://youtu.be/hngtZNNsyM0




