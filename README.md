# FSv2-revision
draft-ietf-idr-flowspec-v2 revision
read me for FSv2 
main branch - text issues with FSv2

branches - FSv2 changes to split document
Draft 1. FSv2 with matches from only IP packets and extended community actions 
    a. Base document with architectural ranges + User ordering for matches + actions 
    b.  Matches only for AFI = 1 (IPv4) or AFI=2 (IPv6) with the SAFIs for normal and VPN
                AFI/SAFI (1/TBD1), AFI/SAFI (2/TBD2), AFI/SAFI-IPv4VPN (1/TBD3), AFI/SAFI-IPv6VPN (2/TBD4) 
                All other s
    c. Ranges of values for matches 
               0 - reserved
			1-63 – IP only 
			64-249 – Non-IP 
			250-255 reserved
			
	d.  Basic DDOS actions 
	
 8 Current actions (with current FSv1 values) 
   02     TAIS: traffic actions per interface group
   06     TRB:  traffic rate limited by bytes
   07     TA: traffic action (terminal/sample)
   08     RDIP: Redirect IPv4
   09     TM: mark DSCP value
   12     TRP: traffic rate limited by packets
   13     RDIPv6: redirect to IPv6
   15     RDIID: redirect to Indirection-id (move from 0x00)

problems to fix in version 1 
   a) dependencies in actions 
   b) interdependencies in actions (conflict) 
   

Draft 2. Wide community use for actions 

Draft 3. FSv2 with outside IP + Extended Community actions + Wide Community  
     a. matches for MPLS, SR-SID, 
     b. Ordered FSv2 action using Extended Community or Wide Community 

Draft 4. L2VPN – with L2/L3 + Wide + Extended 

Draft 5.   Discovering FSv2/FSv1 device capabil
