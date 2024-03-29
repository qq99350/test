 Question #1        A;; o~                                                                                                                                                  Topic  1
 ;; comp~ny needs to ~rchitect ~ hybrid  DNS solution. This solution will use ~n ;;m~zon  Route 53 priv~te hosted zone for the dom~in cloud.ex~mple.com for the resources stored within VPCs. The comp~ny h~s the following  DNS resolution requirements: On-premises systems should be ~ble to resolve ~nd connect to cloud.ex~mple.com. ;;ll VPCs should be ~ble to resolve cloud.ex~mple.com. There is ~lre~dy ~n ;;WS  Direct Connect connection between the on-premises corpor~te network ~nd ;;WS Tr~nsit G~tew~y. Which ~rchitecture should the comp~ny use to meet these requirements with the  HIGHEST perform~nce?
  ;;. ;;ssoci~te the priv~te hosted zone to ~ll the VPCs. Cre~te ~  Route 53 inbound resolver in the sh~red services VPC. ;;tt~ch ~ll VPCs to the tr~nsit g~tew~y ~nd cre~te forw~rding rules in the on-premises  DNS server for cloud.ex~mple.com th~t point to the inbound resolver.
  B. ;;ssoci~te the priv~te hosted zone to ~ll the VPCs.  Deploy ~n ;;m~zon  EC2 condition~l forw~rder in the sh~red services VPC. ;;tt~ch ~ll VPCs to the tr~nsit g~tew~y ~nd cre~te forw~rding rules in the on-premises  DNS server for cloud.ex~mple.com th~t point to the condition~l forw~rder.
  C. ;;ssoci~te the priv~te hosted zone to the sh~red services VPCre~te ~  Route 53 outbound resolver in the sh~red services VP;;tt~ch ~ll VPCs to the tr~nsit g~tew~y ~nd cre~te forw~rding rules in the on-premises  DNS server for cloud.ex~mple.com th~t point to the outbound resolver.
  D. ;;ssoci~te the priv~te hosted zone to the sh~red services VPC. Cre~te ~  Route 53 inbound resolver in the sh~red services VPC. ;;tt~ch the sh~red services VPC to the tr~nsit g~tew~y ~nd cre~te forw~rding rules in the on-premises  DNS server for cloud.ex~mple.com th~t point to the inbound resolver.

 Correct ;;nswer: D
 ;; (86%)                                   14%

 Question #2
 ;; comp~ny is providing we~ther d~t~ over ~  REST-b~sed ;;PI to sever~l customers. The ;;PI is hosted by ;;m~zon ;;PI G~tew~y ~nd is integr~ted with different ;;WS  L~mbd~ functions for e~ch ;;PI oper~tion. The comp~ny uses ;;m~zon  Route 53 for  DNS ~nd h~s cre~ted ~ resource record of we~ther.ex~mple.com. The comp~ny stores d~t~ for the ;;PI in ;;m~zon  Dyn~moDB t~bles. The comp~ny needs ~ solution th~t will give the ;;PI the ~bility to f~il over to ~ different ;;WS  Region. Which solution will meet these requirements?
  ;;.  Deploy ~ new set of  L~mbd~ functions in ~ new  Region. Upd~te the ;;PI G~tew~y ;;PI to use ~n edge-optimized ;;PI endpoint with  L~mbd~ functions from both  Regions ~s t~rgets. Convert the  Dyn~moDB t~bles to glob~l t~bles.
  B.  Deploy ~ new ;;PI G~tew~y ;;PI ~nd  L~mbd~ functions in ~nother  Region. Ch~nge the  Route 53  DNS record to ~ multiv~lue ~nswer. ;;dd both ;;PI G~tew~y ;;PIs to the ~nswer.  En~ble t~rget he~lth monitoring. Convert the  Dyn~moDB t~bles to glob~l t~bles.
  C.  Deploy ~ new ;;PI G~tew~y ;;PI ~nd  L~mbd~ functions in ~nother  Region. Ch~nge the  Route 53  DNS record to ~ f~ilover record.  En~ble t~rget he~lth monitoring. Convert the  Dyn~moDB t~bles to glob~l t~bles.
  D.  Deploy ~ new ;;PI G~tew~y ;;PI in ~ new  Region. Ch~nge the  L~mbd~ functions to glob~l functions. Ch~nge the  Route 53  DNS record to ~ multiv~lue ~nswer. ;;dd both ;;PI G~tew~y ;;PIs to the ~nswer.  En~ble t~rget he~lth monitoring. Convert the  Dyn~moDB t~bles to glob~l t~bles.

 Correct ;;nswer: C
 C (98%)

 Question #3
 ;; comp~ny uses ;;WS Org~niz~tions with ~ single OU n~med  Production to m~n~ge multiple ~ccounts. ;;ll ~ccounts ~re members of the Production OU. ;;dministr~tors use deny list SCPs in the root of the org~niz~tion to m~n~ge ~ccess to restricted services. The comp~ny recently ~cquired ~ new business unit ~nd invited the new unit’s existing ;;WS ~ccount to the org~niz~tion. Once onbo~rded, the ~dministr~tors of the new business unit discovered th~t they ~re not ~ble to upd~te existing ;;WS Con g rules to meet the comp~ny’s policies. Which option will ~llow ~dministr~tors to m~ke ch~nges ~nd continue to enforce the current policies without introducing ~ddition~l long-term m~inten~nce?
  ;;.  Remove the org~niz~tion’s root SCPs th~t limit ~ccess to ;;WS Con g. Cre~te ;;WS Service C~t~log products for the comp~ny’s st~nd~rd ;;WS Con g rules ~nd deploy them throughout the org~niz~tion, including the new ~ccount.
  B. Cre~te ~ tempor~ry OU n~med Onbo~rding for the new ~ccount. ;;pply ~n SCP to the Onbo~rding OU to ~llow ;;WS Con g ~ctions.  Move the new ~ccount to the  Production OU when ~djustments to ;;WS Con g ~re complete.
  C. Convert the org~niz~tion’s root SCPs from deny list SCPs to ~llow list SCPs to ~llow the required services only. Tempor~rily ~pply ~n SCP to the org~niz~tion’s root th~t ~llows ;;WS Con g ~ctions for princip~ls only in the new ~ccount.
  D. Cre~te ~ tempor~ry OU n~med Onbo~rding for the new ~ccount. ;;pply ~n SCP to the Onbo~rding OU to ~llow ;;WS Con g ~ctions.  Move the org~niz~tion’s root SCP to the  Production OU.  Move the new ~ccount to the  Production OU when ~djustments to ;;WS Con g ~re complete.

 Correct ;;nswer: B
 D (82%)                                  Other

 Question #4
 ;; comp~ny is running ~ two-tier web-b~sed ~pplic~tion in ~n on-premises d~t~ center. The ~pplic~tion l~yer consists of ~ single server running ~ st~teful ~pplic~tion. The ~pplic~tion connects to ~  PostgreSQL d~t~b~se running on ~ sep~r~te server. The ~pplic~tion’s user b~se is expected to grow signi c~ntly, so the comp~ny is migr~ting the ~pplic~tion ~nd d~t~b~se to ;;WS. The solution will use ;;m~zon ;;uror~  PostgreSQL, ;;m~zon EC2 ;;uto Sc~ling, ~nd  El~stic  Lo~d  B~l~ncing. Which solution will provide ~ consistent user experience th~t will ~llow the ~pplic~tion ~nd d~t~b~se tiers to sc~le?
  ;;.  En~ble ;;uror~ ;;uto Sc~ling for ;;uror~  Replic~s. Use ~  Network  Lo~d  B~l~ncer with the le~st outst~nding requests routing ~lgorithm ~nd sticky sessions en~bled.
  B.  En~ble ;;uror~ ;;uto Sc~ling for ;;uror~ writers. Use ~n ;;pplic~tion  Lo~d  B~l~ncer with the round robin routing ~lgorithm ~nd sticky sessions en~bled.
  C.  En~ble ;;uror~ ;;uto Sc~ling for ;;uror~  Replic~s. Use ~n ;;pplic~tion  Lo~d  B~l~ncer with the round robin routing ~nd sticky sessions en~bled.
  D.  En~ble ;;uror~ Sc~ling for ;;uror~ writers. Use ~  Network  Lo~d  B~l~ncer with the le~st outst~nding requests routing ~lgorithm ~nd sticky sessions en~bled.

 Correct ;;nswer: C
 C (94%)                                   6%

 Question #5
 ;; comp~ny uses ~ service to collect met~d~t~ from ~pplic~tions th~t the comp~ny hosts on premises. Consumer devices such ~s TVs ~nd internet r~dios ~ccess the ~pplic~tions.  M~ny older devices do not support cert~in  HTTP he~ders ~nd exhibit errors when these he~ders ~re present in responses. The comp~ny h~s con gured ~n on-premises lo~d b~l~ncer to remove the unsupported he~ders from responses sent to older devices, which the comp~ny identi ed by the User-;;gent he~ders. The comp~ny w~nts to migr~te the service to ;;WS, ~dopt serverless technologies, ~nd ret~in the ~bility to support the older devices. The comp~ny h~s ~lre~dy migr~ted the ~pplic~tions into ~ set of ;;WS  L~mbd~ functions. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;m~zon CloudFront distribution for the met~d~t~ service. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Con gure the CloudFront distribution to forw~rd requests to the ;;LB. Con gure the ;;LB to invoke the correct  L~mbd~ function for e~ch type of request. Cre~te ~ CloudFront function to remove the problem~tic he~ders b~sed on the v~lue of the User-;;gent he~der.
  B. Cre~te ~n ;;m~zon ;;PI G~tew~y  REST ;;PI for the met~d~t~ service. Con gure ;;PI G~tew~y to invoke the correct  L~mbd~ function for e~ch type of request.  Modify the def~ult g~tew~y responses to remove the problem~tic he~ders b~sed on the v~lue of the User-;;gent he~der.
  C. Cre~te ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI for the met~d~t~ service. Con gure ;;PI G~tew~y to invoke the correct  L~mbd~ function for e~ch type of request. Cre~te ~ response m~pping templ~te to remove the problem~tic he~ders b~sed on the v~lue of the User-;;gent. ;;ssoci~te the response d~t~ m~pping with the  HTTP ;;PI.
  D. Cre~te ~n ;;m~zon CloudFront distribution for the met~d~t~ service. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Con gure the CloudFront distribution to forw~rd requests to the ;;LB. Con gure the ;;LB to invoke the correct  L~mbd~ function for e~ch type of request. Cre~te ~ L~mbd~@Edge function th~t will remove the problem~tic he~ders in response to viewer requests b~sed on the v~lue of the User-;;gent he~der.

 Correct ;;nswer: B
 ;; (48%)                      D (24%)         B (17%)      10%

 Question #6
 ;; ret~il comp~ny needs to provide ~ series of d~t~  les to ~nother comp~ny, which is its business p~rtner. These  les ~re s~ved in ~n ;;m~zon S3 bucket under ;;ccount ;;, which belongs to the ret~il comp~ny. The business p~rtner comp~ny w~nts one of its  I;;M users, User_D~t~Processor, to ~ccess the  les from its own ;;WS ~ccount (;;ccount  B). Which combin~tion of steps must the comp~nies t~ke so th~t User_D~t~Processor c~n ~ccess the S3 bucket successfully? (Choose two.)
  ;;. Turn on the cross-origin resource sh~ring (CORS) fe~ture for the S3 bucket in ;;ccount ;;.
  B.  In ;;ccount ;;, set the S3 bucket policy to the following:
  C.  In ;;ccount ;;, set the S3 bucket policy to the following:
  D.  In ;;ccount  B, set the permissions of User_D~t~Processor to the following:
  E.  In ;;ccount  B, set the permissions of User_D~t~Processor to the following:

 Correct ;;nswer: D
 C (65%)                                  D (32%)

 Question #7
 ;; comp~ny is running ~ tr~dition~l web ~pplic~tion on ;;m~zon  EC2 inst~nces. The comp~ny needs to ref~ctor the ~pplic~tion ~s microservices th~t run on cont~iners. Sep~r~te versions of the ~pplic~tion exist in two distinct environments: production ~nd testing.  Lo~d for the ~pplic~tion is v~ri~ble, but the minimum lo~d ~nd the m~ximum lo~d ~re known. ;; solutions ~rchitect needs to design the upd~ted ~pplic~tion with ~ serverless ~rchitecture th~t minimizes oper~tion~l complexity. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Uplo~d the cont~iner im~ges to ;;WS  L~mbd~ ~s functions. Con gure ~ concurrency limit for the ~ssoci~ted  L~mbd~ functions to h~ndle the expected pe~k lo~d. Con gure two sep~r~te  L~mbd~ integr~tions within ;;m~zon ;;PI G~tew~y: one for production ~nd one for testing.
  B. Uplo~d the cont~iner im~ges to ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). Con gure two ~uto sc~led ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) clusters with the  F~rg~te l~unch type to h~ndle the expected lo~d.  Deploy t~sks from the  ECR im~ges. Con gure two sep~r~te ;;pplic~tion  Lo~d  B~l~ncers to direct tr~ c to the  ECS clusters.
  C. Uplo~d the cont~iner im~ges to ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). Con gure two ~uto sc~led ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) clusters with the  F~rg~te l~unch type to h~ndle the expected lo~d.  Deploy t~sks from the  ECR im~ges. Con gure two sep~r~te ;;pplic~tion  Lo~d  B~l~ncers to direct tr~ c to the  EKS clusters.
  D. Uplo~d the cont~iner im~ges to ;;WS  El~stic  Be~nst~lk.  In  El~stic  Be~nst~lk, cre~te sep~r~te environments ~nd deployments for production ~nd testing. Con gure two sep~r~te ;;pplic~tion  Lo~d  B~l~ncers to direct tr~ c to the  El~stic  Be~nst~lk deployments.

 Correct ;;nswer: B
 B (84%)                                   Other

 Question #8
 ;; comp~ny h~s ~ multi-tier web ~pplic~tion th~t runs on ~  eet of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The inst~nces ~re in ~n ;;uto Sc~ling group. The ;;LB ~nd the ;;uto Sc~ling group ~re replic~ted in ~ b~ckup ;;WS  Region. The minimum v~lue ~nd the m~ximum v~lue for the ;;uto Sc~ling group ~re set to zero. ;;n ;;m~zon  RDS  Multi-;;Z  DB inst~nce stores the ~pplic~tion’s d~t~. The  DB inst~nce h~s ~ re~d replic~ in the b~ckup  Region. The ~pplic~tion presents ~n endpoint to end users by using ~n ;;m~zon  Route 53 record. The comp~ny needs to reduce its  RTO to less th~n  15 minutes by giving the ~pplic~tion the ~bility to ~utom~tic~lly f~il over to the b~ckup  Region. The comp~ny does not h~ve ~ l~rge enough budget for ~n ~ctive-~ctive str~tegy. Wh~t should ~ solutions ~rchitect recommend to meet these requirements?
  ;;.  Recon gure the ~pplic~tion’s  Route 53 record with ~ l~tency-b~sed routing policy th~t lo~d b~l~nces tr~ c between the two ;;LBs. Cre~te ~n ;;WS  L~mbd~ function in the b~ckup  Region to promote the re~d replic~ ~nd modify the ;;uto Sc~ling group v~lues. Cre~te ~n ;;m~zon CloudW~tch ~l~rm th~t is b~sed on the  HTTPCode_T~rget_5XX_Count metric for the ;;LB in the prim~ry  Region. Con gure the CloudW~tch ~l~rm to invoke the  L~mbd~ function.
  B. Cre~te ~n ;;WS  L~mbd~ function in the b~ckup  Region to promote the re~d replic~ ~nd modify the ;;uto Sc~ling group v~lues. Con gure Route 53 with ~ he~lth check th~t monitors the web ~pplic~tion ~nd sends ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) noti c~tion to the  L~mbd~ function when the he~lth check st~tus is unhe~lthy. Upd~te the ~pplic~tion’s  Route 53 record with ~ f~ilover policy th~t routes tr~ c to the ;;LB in the b~ckup  Region when ~ he~lth check f~ilure occurs.
  C. Con gure the ;;uto Sc~ling group in the b~ckup  Region to h~ve the s~me v~lues ~s the ;;uto Sc~ling group in the prim~ry  Region. Recon gure the ~pplic~tion’s  Route 53 record with ~ l~tency-b~sed routing policy th~t lo~d b~l~nces tr~ c between the two ;;LBs.  Remove the re~d replic~.  Repl~ce the re~d replic~ with ~ st~nd~lone  RDS  DB inst~nce. Con gure Cross-Region  Replic~tion between the  RDS  DB inst~nces by using sn~pshots ~nd ;;m~zon S3.
  D. Con gure ~n endpoint in ;;WS Glob~l ;;cceler~tor with the two ;;LBs ~s equ~l weighted t~rgets. Cre~te ~n ;;WS  L~mbd~ function in the b~ckup  Region to promote the re~d replic~ ~nd modify the ;;uto Sc~ling group v~lues. Cre~te ~n ;;m~zon CloudW~tch ~l~rm th~t is b~sed on the  HTTPCode_T~rget_5XX_Count metric for the ;;LB in the prim~ry  Region. Con gure the CloudW~tch ~l~rm to invoke the  L~mbd~ function.

 Correct ;;nswer: B
 B (100%)

 Question #9
 ;; comp~ny is hosting ~ critic~l ~pplic~tion on ~ single ;;m~zon  EC2 inst~nce. The ~pplic~tion uses ~n ;;m~zon  El~stiC~che for  Redis single-node cluster for ~n in-memory d~t~ store. The ~pplic~tion uses ~n ;;m~zon  RDS for  M~ri~DB  DB inst~nce for ~ rel~tion~l d~t~b~se.  For the ~pplic~tion to function, e~ch piece of the infr~structure must be he~lthy ~nd must be in ~n ~ctive st~te. ;; solutions ~rchitect needs to improve the ~pplic~tion's ~rchitecture so th~t the infr~structure c~n ~utom~tic~lly recover from f~ilure with the le~st possible downtime. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Use ~n  El~stic  Lo~d  B~l~ncer to distribute tr~ c ~cross multiple  EC2 inst~nces.  Ensure th~t the  EC2 inst~nces ~re p~rt of ~n ;;uto Sc~ling group th~t h~s ~ minimum c~p~city of two inst~nces.
  B. Use ~n  El~stic  Lo~d  B~l~ncer to distribute tr~ c ~cross multiple  EC2 inst~nces.  Ensure th~t the  EC2 inst~nces ~re con gured in unlimited mode.
  C.  Modify the  DB inst~nce to cre~te ~ re~d replic~ in the s~me ;;v~il~bility Zone.  Promote the re~d replic~ to be the prim~ry  DB inst~nce in f~ilure scen~rios.
  D.  Modify the  DB inst~nce to cre~te ~  Multi-;;Z deployment th~t extends ~cross two ;;v~il~bility Zones.
  E. Cre~te ~ replic~tion group for the  El~stiC~che for  Redis cluster. Con gure the cluster to use ~n ;;uto Sc~ling group th~t h~s ~ minimum c~p~city of two inst~nces.
  F. Cre~te ~ replic~tion group for the  El~stiC~che for  Redis cluster.  En~ble  Multi-;;Z on the cluster.

 Correct ;;nswer: ;;DF
 ;;DF (97%)

 Question #10
 ;; ret~il comp~ny is oper~ting its ecommerce ~pplic~tion on ;;WS. The ~pplic~tion runs on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d B~l~ncer (;;LB). The comp~ny uses ~n ;;m~zon  RDS  DB inst~nce ~s the d~t~b~se b~ckend. ;;m~zon CloudFront is con gured with one origin th~t points to the ;;LB. St~tic content is c~ched. ;;m~zon  Route 53 is used to host ~ll public zones. ;;fter ~n upd~te of the ~pplic~tion, the ;;LB occ~sion~lly returns ~ 502 st~tus code (B~d G~tew~y) error. The root c~use is m~lformed  HTTP he~ders th~t ~re returned to the ;;LB. The webp~ge returns successfully when ~ solutions ~rchitect relo~ds the webp~ge immedi~tely ~fter the error occurs. While the comp~ny is working on the problem, the solutions ~rchitect needs to provide ~ custom error p~ge inste~d of the st~nd~rd ;;LB error p~ge to visitors. Which combin~tion of steps will meet this requirement with the  LE;;ST ~mount of oper~tion~l overhe~d? (Choose two.)
  ;;. Cre~te ~n ;;m~zon S3 bucket. Con gure the S3 bucket to host ~ st~tic webp~ge. Uplo~d the custom error p~ges to ;;m~zon S3.
  B. Cre~te ~n ;;m~zon CloudW~tch ~l~rm to invoke ~n ;;WS  L~mbd~ function if the ;;LB he~lth check response T~rget.F~iledHe~lthChecks is gre~ter th~n 0. Con gure the  L~mbd~ function to modify the forw~rding rule ~t the ;;LB to point to ~ publicly ~ccessible web server.
  C.  Modify the existing ;;m~zon  Route 53 records by ~dding he~lth checks. Con gure ~ f~llb~ck t~rget if the he~lth check f~ils.  Modify  DNS records to point to ~ publicly ~ccessible webp~ge.
  D. Cre~te ~n ;;m~zon CloudW~tch ~l~rm to invoke ~n ;;WS  L~mbd~ function if the ;;LB he~lth check response  Elb.Intern~lError is gre~ter th~n 0. Con gure the  L~mbd~ function to modify the forw~rding rule ~t the ;;LB to point to ~ public ~ccessible web server.
  E. ;;dd ~ custom error response by con guring ~ CloudFront custom error p~ge.  Modify  DNS records to point to ~ publicly ~ccessible web p~ge.

 Correct ;;nswer: CE
 ;;E (94%)                                   6%

 Question #11
 ;; comp~ny h~s m~ny ;;WS ~ccounts ~nd uses ;;WS Org~niz~tions to m~n~ge ~ll of them. ;; solutions ~rchitect must implement ~ solution th~t the comp~ny c~n use to sh~re ~ common network ~cross multiple ~ccounts. The comp~ny’s infr~structure te~m h~s ~ dedic~ted infr~structure ~ccount th~t h~s ~ VPC. The infr~structure te~m must use this ~ccount to m~n~ge the network.  Individu~l ~ccounts c~nnot h~ve the ~bility to m~n~ge their own networks.  However, individu~l ~ccounts must be ~ble to cre~te ;;WS resources within subnets. Which combin~tion of ~ctions should the solutions ~rchitect perform to meet these requirements? (Choose two.)
  ;;. Cre~te ~ tr~nsit g~tew~y in the infr~structure ~ccount.
  B.  En~ble resource sh~ring from the ;;WS Org~niz~tions m~n~gement ~ccount.
  C. Cre~te VPCs in e~ch ;;WS ~ccount within the org~niz~tion in ;;WS Org~niz~tions. Con gure the VPCs to sh~re the s~me CIDR r~nge ~nd subnets ~s the VPC in the infr~structure ~ccount.  Peer the VPCs in e~ch individu~l ~ccount with the VPC in the infr~structure ~ccount.
  D. Cre~te ~ resource sh~re in ;;WS  Resource ;;ccess  M~n~ger in the infr~structure ~ccount. Select the speci c ;;WS Org~niz~tions OU th~t will use the sh~red network. Select e~ch subnet to ~ssoci~te with the resource sh~re.
  E. Cre~te ~ resource sh~re in ;;WS  Resource ;;ccess  M~n~ger in the infr~structure ~ccount. Select the speci c ;;WS Org~niz~tions OU th~t will use the sh~red network. Select e~ch pre x list to ~ssoci~te with the resource sh~re.

 Correct ;;nswer: ;;D
 BD (88%)                                    12%

 Question #12
 ;; comp~ny w~nts to use ~ third-p~rty softw~re-~s-~-service (S~~S) ~pplic~tion. The third-p~rty S~~S ~pplic~tion is consumed through sever~l ;;PI c~lls. The third-p~rty S~~S ~pplic~tion ~lso runs on ;;WS inside ~ VPC. The comp~ny will consume the third-p~rty S~~S ~pplic~tion from inside ~ VPC. The comp~ny h~s intern~l security policies th~t m~nd~te the use of priv~te connectivity th~t does not tr~verse the internet.  No resources th~t run in the comp~ny VPC ~re ~llowed to be ~ccessed from outside the comp~ny’s VPC. ;;ll permissions must conform to the principles of le~st privilege. Which solution meets these requirements?
  ;;. Cre~te ~n ;;WS  Priv~teLink interf~ce VPC endpoint. Connect this endpoint to the endpoint service th~t the third-p~rty S~~S ~pplic~tion provides. Cre~te ~ security group to limit the ~ccess to the endpoint. ;;ssoci~te the security group with the endpoint.
  B. Cre~te ~n ;;WS Site-to-Site VPN connection between the third-p~rty S~~S ~pplic~tion ~nd the comp~ny VPC. Con gure network ;;CLs to limit ~ccess ~cross the VPN tunnels.
  C. Cre~te ~ VPC peering connection between the third-p~rty S~~S ~pplic~tion ~nd the comp~ny VPUpd~te route t~bles by ~dding the needed routes for the peering connection.
  D. Cre~te ~n ;;WS  Priv~teLink endpoint service. ;;sk the third-p~rty S~~S provider to cre~te ~n interf~ce VPC endpoint for this endpoint service. Gr~nt permissions for the endpoint service to the speci c ~ccount of the third-p~rty S~~S provider.

 Correct ;;nswer: ;;
 ;; (95%)                                     5%

 Question #13
 ;; comp~ny needs to implement ~ p~tching process for its servers. The on-premises servers ~nd ;;m~zon  EC2 inst~nces use ~ v~riety of tools to perform p~tching.  M~n~gement requires ~ single report showing the p~tch st~tus of ~ll the servers ~nd inst~nces. Which set of ~ctions should ~ solutions ~rchitect t~ke to meet these requirements?
  ;;. Use ;;WS Systems  M~n~ger to m~n~ge p~tches on the on-premises servers ~nd  EC2 inst~nces. Use Systems  M~n~ger to gener~te p~tch compli~nce reports.
  B. Use ;;WS OpsWorks to m~n~ge p~tches on the on-premises servers ~nd  EC2 inst~nces. Use ;;m~zon QuickSight integr~tion with OpsWorks to gener~te p~tch compli~nce reports.
  C. Use ~n ;;m~zon  EventBridge rule to ~pply p~tches by scheduling ~n ;;WS Systems  M~n~ger p~tch remedi~tion job. Use ;;m~zon  Inspector to gener~te p~tch compli~nce reports.
  D. Use ;;WS OpsWorks to m~n~ge p~tches on the on-premises servers ~nd  EC2 inst~nces. Use ;;WS X-R~y to post the p~tch st~tus to ;;WS Systems  M~n~ger OpsCenter to gener~te p~tch compli~nce reports.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #14
 ;; comp~ny is running ~n ~pplic~tion on sever~l ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group behind ~n ;;pplic~tion  Lo~d  B~l~ncer. The lo~d on the ~pplic~tion v~ries throughout the d~y, ~nd  EC2 inst~nces ~re sc~led in ~nd out on ~ regul~r b~sis.  Log  les from the  EC2 inst~nces ~re copied to ~ centr~l ;;m~zon S3 bucket every  15 minutes. The security te~m discovers th~t log  les ~re missing from some of the termin~ted  EC2 inst~nces. Which set of ~ctions will ensure th~t log  les ~re copied to the centr~l S3 bucket from the termin~ted  EC2 inst~nces?
  ;;. Cre~te ~ script to copy log  les to ;;m~zon S3, ~nd store the script in ~  le on the  EC2 inst~nce. Cre~te ~n ;;uto Sc~ling lifecycle hook ~nd ~n ;;m~zon  EventBridge rule to detect lifecycle events from the ;;uto Sc~ling group.  Invoke ~n ;;WS  L~mbd~ function on the ~utosc~ling:EC2_INST;;NCE_TERMIN;;TING tr~nsition to send ;;B;;NDON to the ;;uto Sc~ling group to prevent termin~tion, run the script to copy the log  les, ~nd termin~te the inst~nce using the ;;WS SDK.
  B. Cre~te ~n ;;WS Systems  M~n~ger document with ~ script to copy log  les to ;;m~zon S3. Cre~te ~n ;;uto Sc~ling lifecycle hook ~nd ~n ;;m~zon  EventBridge rule to detect lifecycle events from the ;;uto Sc~ling group.  Invoke ~n ;;WS  L~mbd~ function on the ~utosc~ling:EC2_INST;;NCE_TERMIN;;TING tr~nsition to c~ll the ;;WS Systems  M~n~ger ;;PI SendComm~nd oper~tion to run the document to copy the log  les ~nd send CONTINUE to the ;;uto Sc~ling group to termin~te the inst~nce.
  C. Ch~nge the log delivery r~te to every 5 minutes. Cre~te ~ script to copy log  les to ;;m~zon S3, ~nd ~dd the script to  EC2 inst~nce user d~t~. Cre~te ~n ;;m~zon  EventBridge rule to detect  EC2 inst~nce termin~tion.  Invoke ~n ;;WS  L~mbd~ function from the  EventBridge rule th~t uses the ;;WS CLI to run the user-d~t~ script to copy the log  les ~nd termin~te the inst~nce.
  D. Cre~te ~n ;;WS Systems  M~n~ger document with ~ script to copy log  les to ;;m~zon S3. Cre~te ~n ;;uto Sc~ling lifecycle hook th~t publishes ~ mess~ge to ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic.  From the SNS noti c~tion, c~ll the ;;WS Systems M~n~ger ;;PI SendComm~nd oper~tion to run the document to copy the log  les ~nd send ;;B;;NDON to the ;;uto Sc~ling group to termin~te the inst~nce.

 Correct ;;nswer: B
 B (100%)

 Question #15
 ;; comp~ny is using multiple ;;WS ~ccounts. The  DNS records ~re stored in ~ priv~te hosted zone for ;;m~zon  Route 53 in ;;ccount ;;. The comp~ny’s ~pplic~tions ~nd d~t~b~ses ~re running in ;;ccount  B. ;; solutions ~rchitect will deploy ~ two-tier ~pplic~tion in ~ new VPC. To simplify the con gur~tion, the db.ex~mple.com CN;;ME record set for the ;;m~zon  RDS endpoint w~s cre~ted in ~ priv~te hosted zone for ;;m~zon  Route 53. During deployment, the ~pplic~tion f~iled to st~rt. Troubleshooting reve~led th~t db.ex~mple.com is not resolv~ble on the ;;m~zon  EC2 inst~nce. The solutions ~rchitect con rmed th~t the record set w~s cre~ted correctly in  Route 53. Which combin~tion of steps should the solutions ~rchitect t~ke to resolve this issue? (Choose two.)
  ;;.  Deploy the d~t~b~se on ~ sep~r~te  EC2 inst~nce in the new VPC. Cre~te ~ record set for the inst~nce’s priv~te  IP in the priv~te hosted zone.
  B. Use SSH to connect to the ~pplic~tion tier  EC2 inst~nce. ;;dd ~n  RDS endpoint  IP ~ddress to the /etc/resolv.conf  le.
  C. Cre~te ~n ~uthoriz~tion to ~ssoci~te the priv~te hosted zone in ;;ccount ;; with the new VPC in ;;ccount  B.
  D. Cre~te ~ priv~te hosted zone for the ex~mple com dom~in in ;;ccount  B. Con gure  Route 53 replic~tion between ;;WS ~ccounts.
  E. ;;ssoci~te ~ new VPC in ;;ccount  B with ~ hosted zone in ;;ccount ;;.  Delete the ~ssoci~tion ~uthoriz~tion in ;;ccount ;;.

 Correct ;;nswer: BC
 CE (100%)

 Question #16
 ;; comp~ny used ;;m~zon  EC2 inst~nces to deploy ~ web  eet to host ~ blog site. The  EC2 inst~nces ~re behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd ~re con gured in ~n ;;uto Sc~ling group. The web ~pplic~tion stores ~ll blog content on ~n ;;m~zon  EFS volume. The comp~ny recently ~dded ~ fe~ture for bloggers to ~dd video to their posts, ~ttr~cting  10 times the previous user tr~ c. ;;t pe~k times of d~y, users report buffering ~nd timeout issues while ~ttempting to re~ch the site or w~tch videos. Which is the  MOST cost-e cient ~nd sc~l~ble deployment th~t will resolve the issues for users?
  ;;.  Recon gure ;;m~zon  EFS to en~ble m~ximum  I/O.
  B. Upd~te the blog site to use inst~nce store volumes for stor~ge. Copy the site contents to the volumes ~t l~unch ~nd to ;;m~zon S3 ~t shutdown.
  C. Con gure ~n ;;m~zon CloudFront distribution.  Point the distribution to ~n S3 bucket, ~nd migr~te the videos from  EFS to ;;m~zon S3.
  D. Set up ~n ;;m~zon CloudFront distribution for ~ll site contents, ~nd point the distribution ~t the ;;LB.

 Correct ;;nswer: C
 C (98%)

 Question #17
 ;; comp~ny with glob~l o ces h~s ~ single  1 Gbps ;;WS  Direct Connect connection to ~ single ;;WS  Region. The comp~ny’s on-premises network uses the connection to communic~te with the comp~ny’s resources in the ;;WS Cloud. The connection h~s ~ single priv~te virtu~l interf~ce th~t connects to ~ single VPC. ;; solutions ~rchitect must implement ~ solution th~t ~dds ~ redund~nt  Direct Connect connection in the s~me  Region. The solution ~lso must provide connectivity to other  Regions through the s~me p~ir of  Direct Connect connections ~s the comp~ny exp~nds into other  Regions. Which solution meets these requirements?
  ;;.  Provision ~  Direct Connect g~tew~y.  Delete the existing priv~te virtu~l interf~ce from the existing connection. Cre~te the second  Direct Connect connection. Cre~te ~ new priv~te virtu~l interf~ce on e~ch connection, ~nd connect both priv~te virtu~l interf~ces to the  Direct Connect g~tew~y. Connect the  Direct Connect g~tew~y to the single VPC.
  B.  Keep the existing priv~te virtu~l interf~ce. Cre~te the second  Direct Connect connection. Cre~te ~ new priv~te virtu~l interf~ce on the new connection, ~nd connect the new priv~te virtu~l interf~ce to the single VPC.
  C.  Keep the existing priv~te virtu~l interf~ce. Cre~te the second  Direct Connect connection. Cre~te ~ new public virtu~l interf~ce on the new connection, ~nd connect the new public virtu~l interf~ce to the single VPC.
  D.  Provision ~ tr~nsit g~tew~y.  Delete the existing priv~te virtu~l interf~ce from the existing connection. Cre~te the second  Direct Connect connection. Cre~te ~ new priv~te virtu~l interf~ce on e~ch connection, ~nd connect both priv~te virtu~l interf~ces to the tr~nsit g~tew~y. ;;ssoci~te the tr~nsit g~tew~y with the single VPC.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #18
 ;; comp~ny h~s ~ web ~pplic~tion th~t ~llows users to uplo~d short videos. The videos ~re stored on ;;m~zon  EBS volumes ~nd ~n~lyzed by custom recognition softw~re for c~tegoriz~tion. The website cont~ins st~tic content th~t h~s v~ri~ble tr~ c with pe~ks in cert~in months. The ~rchitecture consists of ;;m~zon  EC2 inst~nces running in ~n ;;uto Sc~ling group for the web ~pplic~tion ~nd  EC2 inst~nces running in ~n ;;uto Sc~ling group to process ~n ;;m~zon SQS queue. The comp~ny w~nts to re-~rchitect the ~pplic~tion to reduce oper~tion~l overhe~d using ;;WS m~n~ged services where possible ~nd remove dependencies on third-p~rty softw~re. Which solution meets these requirements?
  ;;. Use ;;m~zon  ECS cont~iners for the web ~pplic~tion ~nd Spot inst~nces for the ;;uto Sc~ling group th~t processes the SQS queue.  Repl~ce the custom softw~re with ;;m~zon  Rekognition to c~tegorize the videos.
  B. Store the uplo~ded videos in ;;m~zon  EFS ~nd mount the  le system to the  EC2 inst~nces for the web ~pplic~tion.  Process the SQS queue with ~n ;;WS  L~mbd~ function th~t c~lls the ;;m~zon  Rekognition ;;PI to c~tegorize the videos.
  C.  Host the web ~pplic~tion in ;;m~zon S3. Store the uplo~ded videos in ;;m~zon S3. Use S3 event noti c~tion to publish events to the SQS queue.  Process the SQS queue with ~n ;;WS  L~mbd~ function th~t c~lls the ;;m~zon  Rekognition ;;PI to c~tegorize the videos.
  D. Use ;;WS  El~stic  Be~nst~lk to l~unch  EC2 inst~nces in ~n ;;uto Sc~ling group for the web ~pplic~tion ~nd l~unch ~ worker environment to process the SQS queue.  Repl~ce the custom softw~re with ;;m~zon  Rekognition to c~tegorize the videos.

 Correct ;;nswer: D
 C (86%)                                   14%

 Question #19
 ;; comp~ny h~s ~ serverless ~pplic~tion comprised of ;;m~zon CloudFront, ;;m~zon ;;PI G~tew~y, ~nd ;;WS  L~mbd~ functions. The current deployment process of the ~pplic~tion code is to cre~te ~ new version number of the  L~mbd~ function ~nd run ~n ;;WS CLI script to upd~te.  If the new function version h~s errors, ~nother CLI script reverts by deploying the previous working version of the function. The comp~ny would like to decre~se the time to deploy new versions of the ~pplic~tion logic provided by the  L~mbd~ functions, ~nd ~lso reduce the time to detect ~nd revert when errors ~re identi ed. How c~n this be ~ccomplished?
  ;;. Cre~te ~nd deploy nested ;;WS CloudForm~tion st~cks with the p~rent st~ck consisting of the ;;WS CloudFront distribution ~nd ;;PI G~tew~y, ~nd the child st~ck cont~ining the  L~mbd~ function.  For ch~nges to  L~mbd~, cre~te ~n ;;WS CloudForm~tion ch~nge set ~nd deploy; if errors ~re triggered, revert the ;;WS CloudForm~tion ch~nge set to the previous version.
  B. Use ;;WS S;;M ~nd built-in ;;WS CodeDeploy to deploy the new  L~mbd~ version, gr~du~lly shift tr~ c to the new version, ~nd use pre-tr~ c ~nd post-tr~ c test functions to verify code.  Rollb~ck if ;;m~zon CloudW~tch ~l~rms ~re triggered.
  C.  Ref~ctor the ;;WS CLI scripts into ~ single script th~t deploys the new  L~mbd~ version. When deployment is completed, the script tests execute.  If errors ~re detected, revert to the previous  L~mbd~ version.
  D. Cre~te ~nd deploy ~n ;;WS CloudForm~tion st~ck th~t consists of ~ new ;;PI G~tew~y endpoint th~t references the new  L~mbd~ version. Ch~nge the CloudFront origin to the new ;;PI G~tew~y endpoint, monitor errors ~nd if detected, ch~nge the ;;WS CloudFront origin to the previous ;;PI G~tew~y endpoint.

 Correct ;;nswer: B
 B (100%)

 Question #20
 ;; comp~ny is pl~nning to store ~ l~rge number of ~rchived documents ~nd m~ke the documents ~v~il~ble to employees through the corpor~te intr~net.  Employees will ~ccess the system by connecting through ~ client VPN service th~t is ~tt~ched to ~ VPC. The d~t~ must not be ~ccessible to the public. The documents th~t the comp~ny is storing ~re copies of d~t~ th~t is held on physic~l medi~ elsewhere. The number of requests will be low. ;;v~il~bility ~nd speed of retriev~l ~re not concerns of the comp~ny. Which solution will meet these requirements ~t the  LOWEST cost?
  ;;. Cre~te ~n ;;m~zon S3 bucket. Con gure the S3 bucket to use the S3 One Zone-Infrequent ;;ccess (S3 One Zone-I;;) stor~ge cl~ss ~s def~ult. Con gure the S3 bucket for website hosting. Cre~te ~n S3 interf~ce endpoint. Con gure the S3 bucket to ~llow ~ccess only through th~t endpoint.
  B.  L~unch ~n ;;m~zon  EC2 inst~nce th~t runs ~ web server. ;;tt~ch ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system to store the ~rchived d~t~ in the  EFS One Zone-Infrequent ;;ccess (EFS One Zone-I;;) stor~ge cl~ss Con gure the inst~nce security groups to ~llow ~ccess only from priv~te networks.
  C.  L~unch ~n ;;m~zon  EC2 inst~nce th~t runs ~ web server ;;tt~ch ~n ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume to store the ~rchived d~t~. Use the Cold  HDD (sc1) volume type. Con gure the inst~nce security groups to ~llow ~ccess only from priv~te networks.
  D. Cre~te ~n ;;m~zon S3 bucket. Con gure the S3 bucket to use the S3 Gl~cier  Deep ;;rchive stor~ge cl~ss ~s def~ult. Con gure the S3 bucket for website hosting. Cre~te ~n S3 interf~ce endpoint. Con gure the S3 bucket to ~llow ~ccess only through th~t endpoint.

 Correct ;;nswer: D
 ;; (64%)                                  D (35%)

 Question #21
 ;; comp~ny is using ~n on-premises ;;ctive  Directory service for user ~uthentic~tion. The comp~ny w~nts to use the s~me ~uthentic~tion service to sign in to the comp~ny’s ;;WS ~ccounts, which ~re using ;;WS Org~niz~tions. ;;WS Site-to-Site VPN connectivity ~lre~dy exists between the on- premises environment ~nd ~ll the comp~ny’s ;;WS ~ccounts. The comp~ny’s security policy requires condition~l ~ccess to the ~ccounts b~sed on user groups ~nd roles. User identities must be m~n~ged in ~ single loc~tion. Which solution will meet these requirements?
  ;;. Con gure ;;WS  I;;M  Identity Center (;;WS Single Sign-On) to connect to ;;ctive  Directory by using S;;ML 2.0.  En~ble ~utom~tic provisioning by using the System for Cross-dom~in  Identity  M~n~gement (SCIM) v2.0 protocol. Gr~nt ~ccess to the ;;WS ~ccounts by using ~ttribute-b~sed ~ccess controls (;;B;;Cs).
  B. Con gure ;;WS  I;;M  Identity Center (;;WS Single Sign-On) by using  I;;M  Identity Center ~s ~n identity source.  En~ble ~utom~tic provisioning by using the System for Cross-dom~in  Identity  M~n~gement (SCIM) v2.0 protocol. Gr~nt ~ccess to the ;;WS ~ccounts by using  I;;M  Identity Center permission sets.
  C.  In one of the comp~ny’s ;;WS ~ccounts, con gure ;;WS  Identity ~nd ;;ccess  M~n~gement (I;;M) to use ~ S;;ML 2.0 identity provider. Provision  I;;M users th~t ~re m~pped to the feder~ted users. Gr~nt ~ccess th~t corresponds to ~ppropri~te groups in ;;ctive  Directory. Gr~nt ~ccess to the required ;;WS ~ccounts by using cross-~ccount  I;;M users.
  D.  In one of the comp~ny’s ;;WS ~ccounts, con gure ;;WS  Identity ~nd ;;ccess  M~n~gement (I;;M) to use ~n OpenID Connect (OIDC) identity provider.  Provision  I;;M roles th~t gr~nt ~ccess to the ;;WS ~ccount for the feder~ted users th~t correspond to ~ppropri~te groups in ;;ctive Directory. Gr~nt ~ccess to the required ;;WS ~ccounts by using cross-~ccount  I;;M roles.

 Correct ;;nswer: D
 ;; (77%)                              9%       9%

 Question #22
 ;; softw~re comp~ny h~s deployed ~n ~pplic~tion th~t consumes ~  REST ;;PI by using ;;m~zon ;;PI G~tew~y, ;;WS  L~mbd~ functions, ~nd ~n ;;m~zon  Dyn~moDB t~ble. The ~pplic~tion is showing ~n incre~se in the number of errors during  PUT requests.  Most of the  PUT c~lls come from ~ sm~ll number of clients th~t ~re ~uthentic~ted with speci c ;;PI keys. ;; solutions ~rchitect h~s identi ed th~t ~ l~rge number of the  PUT requests origin~te from one client. The ;;PI is noncritic~l, ~nd clients c~n toler~te retries of unsuccessful c~lls.  However, the errors ~re displ~yed to customers ~nd ~re c~using d~m~ge to the ;;PI’s reput~tion. Wh~t should the solutions ~rchitect recommend to improve the customer experience?
  ;;.  Implement retry logic with exponenti~l b~ckoff ~nd irregul~r v~ri~tion in the client ~pplic~tion.  Ensure th~t the errors ~re c~ught ~nd h~ndled with descriptive error mess~ges.
  B.  Implement ;;PI throttling through ~ us~ge pl~n ~t the ;;PI G~tew~y level.  Ensure th~t the client ~pplic~tion h~ndles code 429 replies without error.
  C. Turn on ;;PI c~ching to enh~nce responsiveness for the production st~ge.  Run  10-minute lo~d tests. Verify th~t the c~che c~p~city is ~ppropri~te for the worklo~d.
  D.  Implement reserved concurrency ~t the  L~mbd~ function level to provide the resources th~t ~re needed during sudden incre~ses in tr~ c.

 Correct ;;nswer: B
 B (71%)                                 ;; (28%)

 Question #23
 ;; comp~ny is running ~ d~t~-intensive ~pplic~tion on ;;WS. The ~pplic~tion runs on ~ cluster of hundreds of ;;m~zon  EC2 inst~nces. ;; sh~red  le system ~lso runs on sever~l  EC2 inst~nces th~t store 200 TB of d~t~. The ~pplic~tion re~ds ~nd modi es the d~t~ on the sh~red  le system ~nd gener~tes ~ report. The job runs once monthly, re~ds ~ subset of the  les from the sh~red  le system, ~nd t~kes ~bout 72 hours to complete. The compute inst~nces sc~le in ~n ;;uto Sc~ling group, but the inst~nces th~t host the sh~red  le system run continuously. The compute ~nd stor~ge inst~nces ~re ~ll in the s~me ;;WS  Region. ;; solutions ~rchitect needs to reduce costs by repl~cing the sh~red  le system inst~nces. The  le system must provide high perform~nce ~ccess to the needed d~t~ for the dur~tion of the 72-hour run. Which solution will provide the  L;;RGEST over~ll cost reduction while meeting these requirements?
  ;;.  Migr~te the d~t~ from the existing sh~red  le system to ~n ;;m~zon S3 bucket th~t uses the S3  Intelligent-Tiering stor~ge cl~ss.  Before the job runs e~ch month, use ;;m~zon  FSx for  Lustre to cre~te ~ new  le system with the d~t~ from ;;m~zon S3 by using l~zy lo~ding. Use the new  le system ~s the sh~red stor~ge for the dur~tion of the job.  Delete the  le system when the job is complete.
  B.  Migr~te the d~t~ from the existing sh~red  le system to ~ l~rge ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume with  Multi-;;tt~ch en~bled. ;;tt~ch the  EBS volume to e~ch of the inst~nces by using ~ user d~t~ script in the ;;uto Sc~ling group l~unch templ~te. Use the  EBS volume ~s the sh~red stor~ge for the dur~tion of the job.  Det~ch the  EBS volume when the job is complete
  C.  Migr~te the d~t~ from the existing sh~red  le system to ~n ;;m~zon S3 bucket th~t uses the S3 St~nd~rd stor~ge cl~ss.  Before the job runs e~ch month, use ;;m~zon  FSx for  Lustre to cre~te ~ new  le system with the d~t~ from ;;m~zon S3 by using b~tch lo~ding. Use the new  le system ~s the sh~red stor~ge for the dur~tion of the job.  Delete the  le system when the job is complete.
  D.  Migr~te the d~t~ from the existing sh~red  le system to ~n ;;m~zon S3 bucket.  Before the job runs e~ch month, use ;;WS Stor~ge G~tew~y to cre~te ~  le g~tew~y with the d~t~ from ;;m~zon S3. Use the  le g~tew~y ~s the sh~red stor~ge for the job.  Delete the  le g~tew~y when the job is complete.

 Correct ;;nswer: D
 ;; (89%)                                   11%

 Question #24
 ;; comp~ny is developing ~ new service th~t will be ~ccessed using TCP on ~ st~tic port. ;; solutions ~rchitect must ensure th~t the service is highly ~v~il~ble, h~s redund~ncy ~cross ;;v~il~bility Zones, ~nd is ~ccessible using the  DNS n~me my.service.com, which is publicly ~ccessible. The service must use  xed ~ddress ~ssignments so other comp~nies c~n ~dd the ~ddresses to their ~llow lists. ;;ssuming th~t resources ~re deployed in multiple ;;v~il~bility Zones in ~ single  Region, which solution will meet these requirements?
  ;;. Cre~te ;;m~zon  EC2 inst~nces with ~n  El~stic  IP ~ddress for e~ch inst~nce. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) ~nd expose the st~tic TCP port.  Register  EC2 inst~nces with the  NLB. Cre~te ~ new n~me server record set n~med my.service.com, ~nd ~ssign the  El~stic  IP ~ddresses of the  EC2 inst~nces to the record set.  Provide the  El~stic  IP ~ddresses of the  EC2 inst~nces to the other comp~nies to ~dd to their ~llow lists.
  B. Cre~te ~n ;;m~zon  ECS cluster ~nd ~ service de nition for the ~pplic~tion. Cre~te ~nd ~ssign public  IP ~ddresses for the  ECS cluster. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) ~nd expose the TCP port. Cre~te ~ t~rget group ~nd ~ssign the  ECS cluster n~me to the  NLCre~te ~ new ;; record set n~med my.service.com, ~nd ~ssign the public  IP ~ddresses of the  ECS cluster to the record set.  Provide the public  IP ~ddresses of the  ECS cluster to the other comp~nies to ~dd to their ~llow lists.
  C. Cre~te ;;m~zon  EC2 inst~nces for the service. Cre~te one  El~stic  IP ~ddress for e~ch ;;v~il~bility Zone. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) ~nd expose the ~ssigned TCP port. ;;ssign the  El~stic  IP ~ddresses to the  NLB for e~ch ;;v~il~bility Zone. Cre~te ~ t~rget group ~nd register the  EC2 inst~nces with the  NLB. Cre~te ~ new ;; (~li~s) record set n~med my.service.com, ~nd ~ssign the  NLB  DNS n~me to the record set.
  D. Cre~te ~n ;;m~zon  ECS cluster ~nd ~ service de nition for the ~pplic~tion. Cre~te ~nd ~ssign public  IP ~ddress for e~ch host in the cluster. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd expose the st~tic TCP port. Cre~te ~ t~rget group ~nd ~ssign the  ECS service de nition n~me to the ;;LB. Cre~te ~ new CN;;ME record set ~nd ~ssoci~te the public  IP ~ddresses to the record set.  Provide the  El~stic  IP ~ddresses of the ;;m~zon  EC2 inst~nces to the other comp~nies to ~dd to their ~llow lists.

 Correct ;;nswer: C
 C (100%)

 Question #25
 ;; comp~ny uses ~n on-premises d~t~ ~n~lytics pl~tform. The system is highly ~v~il~ble in ~ fully redund~nt con gur~tion ~cross  12 servers in the comp~ny’s d~t~ center. The system runs scheduled jobs, both hourly ~nd d~ily, in ~ddition to one-time requests from users. Scheduled jobs c~n t~ke between 20 minutes ~nd 2 hours to  nish running ~nd h~ve tight SL;;s. The scheduled jobs ~ccount for 65% of the system us~ge. User jobs typic~lly  nish running in less th~n 5 minutes ~nd h~ve no SL;;. The user jobs ~ccount for 35% of system us~ge.  During system f~ilures, scheduled jobs must continue to meet SL;;s.  However, user jobs c~n be del~yed. ;; solutions ~rchitect needs to move the system to ;;m~zon  EC2 inst~nces ~nd ~dopt ~ consumption-b~sed model to reduce costs with no long- term commitments. The solution must m~int~in high ~v~il~bility ~nd must not ~ffect the SL;;s. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Split the  12 inst~nces ~cross two ;;v~il~bility Zones in the chosen ;;WS  Region.  Run two inst~nces in e~ch ;;v~il~bility Zone ~s On-Dem~nd Inst~nces with C~p~city  Reserv~tions.  Run four inst~nces in e~ch ;;v~il~bility Zone ~s Spot  Inst~nces.
  B. Split the  12 inst~nces ~cross three ;;v~il~bility Zones in the chosen ;;WS  Region.  In one of the ;;v~il~bility Zones, run ~ll four inst~nces ~s On-Dem~nd  Inst~nces with C~p~city  Reserv~tions.  Run the rem~ining inst~nces ~s Spot  Inst~nces.
  C. Split the  12 inst~nces ~cross three ;;v~il~bility Zones in the chosen ;;WS  Region.  Run two inst~nces in e~ch ;;v~il~bility Zone ~s On-Dem~nd Inst~nces with ~ S~vings  Pl~n.  Run two inst~nces in e~ch ;;v~il~bility Zone ~s Spot  Inst~nces.
  D. Split the  12 inst~nces ~cross three ;;v~il~bility Zones in the chosen ;;WS  Region.  Run three inst~nces in e~ch ;;v~il~bility Zone ~s On- Dem~nd  Inst~nces with C~p~city  Reserv~tions.  Run one inst~nce in e~ch ;;v~il~bility Zone ~s ~ Spot  Inst~nce.

 Correct ;;nswer: C
 D (91%)                                    9%

 Question #26
 ;; security engineer determined th~t ~n existing ~pplic~tion retrieves credenti~ls to ~n ;;m~zon  RDS for  MySQL d~t~b~se from ~n encrypted  le in ;;m~zon S3.  For the next version of the ~pplic~tion, the security engineer w~nts to implement the following ~pplic~tion design ch~nges to improve security: The d~t~b~se must use strong, r~ndomly gener~ted p~sswords stored in ~ secure ;;WS m~n~ged service. The ~pplic~tion resources must be deployed through ;;WS CloudForm~tion. The ~pplic~tion must rot~te credenti~ls for the d~t~b~se every 90 d~ys. ;; solutions ~rchitect will gener~te ~ CloudForm~tion templ~te to deploy the ~pplic~tion. Which resources speci ed in the CloudForm~tion templ~te will meet the security engineer’s requirements with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;. Gener~te the d~t~b~se p~ssword ~s ~ secret resource using ;;WS Secrets  M~n~ger. Cre~te ~n ;;WS  L~mbd~ function resource to rot~te the d~t~b~se p~ssword. Specify ~ Secrets  M~n~ger  Rot~tionSchedule resource to rot~te the d~t~b~se p~ssword every 90 d~ys.
  B. Gener~te the d~t~b~se p~ssword ~s ~ SecureString p~r~meter type using ;;WS Systems  M~n~ger  P~r~meter Store. Cre~te ~n ;;WS  L~mbd~ function resource to rot~te the d~t~b~se p~ssword. Specify ~  P~r~meter Store  Rot~tionSchedule resource to rot~te the d~t~b~se p~ssword every 90 d~ys.
  C. Gener~te the d~t~b~se p~ssword ~s ~ secret resource using ;;WS Secrets  M~n~ger. Cre~te ~n ;;WS  L~mbd~ function resource to rot~te the d~t~b~se p~ssword. Cre~te ~n ;;m~zon  EventBridge scheduled rule resource to trigger the  L~mbd~ function p~ssword rot~tion every 90 d~ys.
  D. Gener~te the d~t~b~se p~ssword ~s ~ SecureString p~r~meter type using ;;WS Systems  M~n~ger  P~r~meter Store. Specify ~n ;;WS ;;ppSync D~t~Source resource to ~utom~tic~lly rot~te the d~t~b~se p~ssword every 90 d~ys.

 Correct ;;nswer: B
 ;; (100%)

 Question #27
 ;; comp~ny is storing d~t~ in sever~l ;;m~zon  Dyn~moDB t~bles. ;; solutions ~rchitect must use ~ serverless ~rchitecture to m~ke the d~t~ ~ccessible publicly through ~ simple ;;PI over  HTTPS. The solution must sc~le ~utom~tic~lly in response to dem~nd. Which solutions meet these requirements? (Choose two.)
  ;;. Cre~te ~n ;;m~zon ;;PI G~tew~y  REST ;;PI. Con gure this ;;PI with direct integr~tions to  Dyn~moDB by using ;;PI G~tew~y’s ;;WS integr~tion type.
  B. Cre~te ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI. Con gure this ;;PI with direct integr~tions to  Dyn~mo  DB by using ;;PI G~tew~y’s ;;WS integr~tion type.
  C. Cre~te ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI. Con gure this ;;PI with integr~tions to ;;WS  L~mbd~ functions th~t return d~t~ from the Dyn~moDB t~bles.
  D. Cre~te ~n ~cceler~tor in ;;WS Glob~l ;;cceler~tor. Con gure this ~cceler~tor with ;;WS  L~mbd~@Edge function integr~tions th~t return d~t~ from the  Dyn~moDB t~bles.
  E. Cre~te ~  Network  Lo~d  B~l~ncer. Con gure listener rules to forw~rd requests to the ~ppropri~te ;;WS  L~mbd~ functions.

 Correct ;;nswer: CD
 ;;C (79%)                               11%      5%

 Question #28
 ;; comp~ny h~s registered  10 new dom~in n~mes. The comp~ny uses the dom~ins for online m~rketing. The comp~ny needs ~ solution th~t will redirect online visitors to ~ speci c URL for e~ch dom~in. ;;ll dom~ins ~nd t~rget URLs ~re de ned in ~ JSON document. ;;ll  DNS records ~re m~n~ged by ;;m~zon  Route 53. ;; solutions ~rchitect must implement ~ redirect service th~t ~ccepts  HTTP ~nd  HTTPS requests. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements with the  LE;;ST ~mount of oper~tion~l effort? (Choose three.)
  ;;. Cre~te ~ dyn~mic webp~ge th~t runs on ~n ;;m~zon  EC2 inst~nce. Con gure the webp~ge to use the JSON document in combin~tion with the event mess~ge to look up ~nd respond with ~ redirect URL.
  B. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer th~t includes  HTTP ~nd  HTTPS listeners.
  C. Cre~te ~n ;;WS  L~mbd~ function th~t uses the JSON document in combin~tion with the event mess~ge to look up ~nd respond with ~ redirect URL.
  D. Use ~n ;;m~zon ;;PI G~tew~y ;;PI with ~ custom dom~in to publish ~n ;;WS  L~mbd~ function.
  E. Cre~te ~n ;;m~zon CloudFront distribution.  Deploy ~  L~mbd~@Edge function.
  F. Cre~te ~n SSL certi c~te by using ;;WS Certi c~te  M~n~ger (;;CM).  Include the dom~ins ~s Subject ;;ltern~tive  N~mes.

 Correct ;;nswer: BCF
 CEF (57%)                         BCF (27%)          Other

 Question #29
 ;; comp~ny th~t h~s multiple ;;WS ~ccounts is using ;;WS Org~niz~tions. The comp~ny’s ;;WS ~ccounts host VPCs, ;;m~zon  EC2 inst~nces, ~nd cont~iners. The comp~ny’s compli~nce te~m h~s deployed ~ security tool in e~ch VPC where the comp~ny h~s deployments. The security tools run on  EC2 inst~nces ~nd send inform~tion to the ;;WS ~ccount th~t is dedic~ted for the compli~nce te~m. The comp~ny h~s t~gged ~ll the compli~nce- rel~ted resources with ~ key of “costCenter” ~nd ~ v~lue or “compli~nce”. The comp~ny w~nts to identify the cost of the security tools th~t ~re running on the  EC2 inst~nces so th~t the comp~ny c~n ch~rge the compli~nce te~m’s ;;WS ~ccount. The cost c~lcul~tion must be ~s ~ccur~te ~s possible. Wh~t should ~ solutions ~rchitect do to meet these requirements?
  ;;.  In the m~n~gement ~ccount of the org~niz~tion, ~ctiv~te the costCenter user-de ned t~g. Con gure monthly ;;WS Cost ~nd Us~ge  Reports to s~ve to ~n ;;m~zon S3 bucket in the m~n~gement ~ccount. Use the t~g bre~kdown in the report to obt~in the tot~l cost for the costCenter t~gged resources.
  B.  In the member ~ccounts of the org~niz~tion, ~ctiv~te the costCenter user-de ned t~g. Con gure monthly ;;WS Cost ~nd Us~ge  Reports to s~ve to ~n ;;m~zon S3 bucket in the m~n~gement ~ccount. Schedule ~ monthly ;;WS  L~mbd~ function to retrieve the reports ~nd c~lcul~te the tot~l cost for the costCenter t~gged resources.
  C.  In the member ~ccounts of the org~niz~tion ~ctiv~te the costCenter user-de ned t~g.  From the m~n~gement ~ccount, schedule ~ monthly ;;WS Cost ~nd Us~ge  Report. Use the t~g bre~kdown in the report to c~lcul~te the tot~l cost for the costCenter t~gged resources.
  D. Cre~te ~ custom report in the org~niz~tion view in ;;WS Trusted ;;dvisor. Con gure the report to gener~te ~ monthly billing summ~ry for the costCenter t~gged resources in the compli~nce te~m’s ;;WS ~ccount.

 Correct ;;nswer: ;;
 ;; (94%)                                   6%

 Question #30
 ;; comp~ny h~s 50 ;;WS ~ccounts th~t ~re members of ~n org~niz~tion in ;;WS Org~niz~tions.  E~ch ~ccount cont~ins multiple VPCs. The comp~ny w~nts to use ;;WS Tr~nsit G~tew~y to est~blish connectivity between the VPCs in e~ch member ~ccount.  E~ch time ~ new member ~ccount is cre~ted, the comp~ny w~nts to ~utom~te the process of cre~ting ~ new VPC ~nd ~ tr~nsit g~tew~y ~tt~chment. Which combin~tion of steps will meet these requirements? (Choose two.)
  ;;.  From the m~n~gement ~ccount, sh~re the tr~nsit g~tew~y with member ~ccounts by using ;;WS  Resource ;;ccess  M~n~ger.
  B.  From the m~n~gement ~ccount, sh~re the tr~nsit g~tew~y with member ~ccounts by using ~n ;;WS Org~niz~tions SCP.
  C.  L~unch ~n ;;WS CloudForm~tion st~ck set from the m~n~gement ~ccount th~t ~utom~tic~lly cre~tes ~ new VPC ~nd ~ VPC tr~nsit g~tew~y ~tt~chment in ~ member ~ccount. ;;ssoci~te the ~tt~chment with the tr~nsit g~tew~y in the m~n~gement ~ccount by using the tr~nsit g~tew~y ID.
  D.  L~unch ~n ;;WS CloudForm~tion st~ck set from the m~n~gement ~ccount th~t ~utom~tic~lly cre~tes ~ new VPC ~nd ~ peering tr~nsit g~tew~y ~tt~chment in ~ member ~ccount. Sh~re the ~tt~chment with the tr~nsit g~tew~y in the m~n~gement ~ccount by using ~ tr~nsit g~tew~y service-linked role.
  E.  From the m~n~gement ~ccount, sh~re the tr~nsit g~tew~y with member ~ccounts by using ;;WS Service C~t~log.

 Correct ;;nswer: ;;C
 ;;C (100%)

 Question #31
 ;;n enterprise comp~ny w~nts to ~llow its developers to purch~se third-p~rty softw~re through ;;WS  M~rketpl~ce. The comp~ny uses ~n ;;WS Org~niz~tions ~ccount structure with full fe~tures en~bled, ~nd h~s ~ sh~red services ~ccount in e~ch org~niz~tion~l unit (OU) th~t will be used by procurement m~n~gers. The procurement te~m’s policy indic~tes th~t developers should be ~ble to obt~in third-p~rty softw~re from ~n ~pproved list only ~nd use  Priv~te  M~rketpl~ce in ;;WS  M~rketpl~ce to ~chieve this requirement. The procurement te~m w~nts ~dministr~tion of  Priv~te M~rketpl~ce to be restricted to ~ role n~med procurement-m~n~ger-role, which could be ~ssumed by procurement m~n~gers. Other  I;;M users, groups, roles, ~nd ~ccount ~dministr~tors in the comp~ny should be denied  Priv~te  M~rketpl~ce ~dministr~tive ~ccess. Wh~t is the  MOST e cient w~y to design ~n ~rchitecture to meet these requirements?
  ;;. Cre~te ~n  I;;M role n~med procurement-m~n~ger-role in ~ll ;;WS ~ccounts in the org~niz~tion. ;;dd the  PowerUser;;ccess m~n~ged policy to the role. ;;pply ~n inline policy to ~ll  I;;M users ~nd roles in every ;;WS ~ccount to deny permissions on the ;;WSPriv~teM~rketpl~ce;;dminFull;;ccess m~n~ged policy.
  B. Cre~te ~n  I;;M role n~med procurement-m~n~ger-role in ~ll ;;WS ~ccounts in the org~niz~tion. ;;dd the ;;dministr~tor;;ccess m~n~ged policy to the role.  De ne ~ permissions bound~ry with the ;;WSPriv~teM~rketpl~ce;;dminFull;;ccess m~n~ged policy ~nd ~tt~ch it to ~ll the developer roles.
  C. Cre~te ~n  I;;M role n~med procurement-m~n~ger-role in ~ll the sh~red services ~ccounts in the org~niz~tion. ;;dd the ;;WSPriv~teM~rketpl~ce;;dminFull;;ccess m~n~ged policy to the role. Cre~te ~n org~niz~tion root-level SCP to deny permissions to ~dminister Priv~te  M~rketpl~ce to everyone except the role n~med procurement-m~n~ger-role. Cre~te ~nother org~niz~tion root-level SCP to deny permissions to cre~te ~n  I;;M role n~med procurement-m~n~ger-role to everyone in the org~niz~tion.
  D. Cre~te ~n  I;;M role n~med procurement-m~n~ger-role in ~ll ;;WS ~ccounts th~t will be used by developers. ;;dd the ;;WSPriv~teM~rketpl~ce;;dminFull;;ccess m~n~ged policy to the role. Cre~te ~n SCP in Org~niz~tions to deny permissions to ~dminister Priv~te  M~rketpl~ce to everyone except the role n~med procurement-m~n~ger-role. ;;pply the SCP to ~ll the sh~red services ~ccounts in the org~niz~tion.

 Correct ;;nswer: D
 C (93%)                                    8%

 Question #32
 ;; comp~ny is in the process of implementing ;;WS Org~niz~tions to constr~in its developers to use only ;;m~zon  EC2, ;;m~zon S3, ~nd ;;m~zon Dyn~moDB. The developers ~ccount resides in ~ dedic~ted org~niz~tion~l unit (OU). The solutions ~rchitect h~s implemented the following SCP on the developers ~ccount: When this policy is deployed,  I;;M users in the developers ~ccount ~re still ~ble to use ;;WS services th~t ~re not listed in the policy. Wh~t should the solutions ~rchitect do to elimin~te the developers’ ~bility to use services outside the scope of this policy?
  ;;. Cre~te ~n explicit deny st~tement for e~ch ;;WS service th~t should be constr~ined.
  B.  Remove the  Full;;WS;;ccess SCP from the developers ~ccount’s OU.
  C.  Modify the  Full;;WS;;ccess SCP to explicitly deny ~ll services.
  D. ;;dd ~n explicit deny st~tement using ~ wildc~rd to the end of the SCP.

 Correct ;;nswer: ;;
 B (81%)                                    Other

 Question #33
 ;; comp~ny is hosting ~ monolithic  REST-b~sed ;;PI for ~ mobile ~pp on  ve ;;m~zon  EC2 inst~nces in public subnets of ~ VPC.  Mobile clients connect to the ;;PI by using ~ dom~in n~me th~t is hosted on ;;m~zon  Route 53. The comp~ny h~s cre~ted ~  Route 53 multiv~lue ~nswer routing policy with the  IP ~ddresses of ~ll the  EC2 inst~nces.  Recently, the ~pp h~s been overwhelmed by l~rge ~nd sudden incre~ses to tr~ c. The ~pp h~s not been ~ble to keep up with the tr~ c. ;; solutions ~rchitect needs to implement ~ solution so th~t the ~pp c~n h~ndle the new ~nd v~rying lo~d. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Sep~r~te the ;;PI into individu~l ;;WS  L~mbd~ functions. Con gure ~n ;;m~zon ;;PI G~tew~y  REST ;;PI with  L~mbd~ integr~tion for the b~ckend. Upd~te the  Route 53 record to point to the ;;PI G~tew~y ;;PI.
  B. Cont~inerize the ;;PI logic. Cre~te ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster.  Run the cont~iners in the cluster by using ;;m~zon  EC2. Cre~te ~  Kubernetes ingress. Upd~te the  Route 53 record to point to the  Kubernetes ingress.
  C. Cre~te ~n ;;uto Sc~ling group.  Pl~ce ~ll the  EC2 inst~nces in the ;;uto Sc~ling group. Con gure the ;;uto Sc~ling group to perform sc~ling ~ctions th~t ~re b~sed on CPU utiliz~tion. Cre~te ~n ;;WS  L~mbd~ function th~t re~cts to ;;uto Sc~ling group ch~nges ~nd upd~tes the  Route 53 record.
  D. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) in front of the ;;PI.  Move the  EC2 inst~nces to priv~te subnets in the VPC. ;;dd the  EC2 inst~nces ~s t~rgets for the ;;LB. Upd~te the  Route 53 record to point to the ;;LB.

 Correct ;;nswer: D
 ;; (54%)                         D (25%)            C (22%)

 Question #34
 ;; comp~ny h~s cre~ted ~n OU in ;;WS Org~niz~tions for e~ch of its engineering te~ms.  E~ch OU owns multiple ;;WS ~ccounts. The org~niz~tion h~s hundreds of ;;WS ~ccounts. ;; solutions ~rchitect must design ~ solution so th~t e~ch OU c~n view ~ bre~kdown of us~ge costs ~cross its ;;WS ~ccounts. Which solution meets these requirements?
  ;;. Cre~te ~n ;;WS Cost ~nd Us~ge  Report (CUR) for e~ch OU by using ;;WS  Resource ;;ccess  M~n~ger. ;;llow e~ch te~m to visu~lize the CUR through ~n ;;m~zon QuickSight d~shbo~rd.
  B. Cre~te ~n ;;WS Cost ~nd Us~ge  Report (CUR) from the ;;WS Org~niz~tions m~n~gement ~ccount. ;;llow e~ch te~m to visu~lize the CUR through ~n ;;m~zon QuickSight d~shbo~rd.
  C. Cre~te ~n ;;WS Cost ~nd Us~ge  Report (CUR) in e~ch ;;WS Org~niz~tions member ~ccount. ;;llow e~ch te~m to visu~lize the CUR through ~n ;;m~zon QuickSight d~shbo~rd.
  D. Cre~te ~n ;;WS Cost ~nd Us~ge  Report (CUR) by using ;;WS Systems  M~n~ger. ;;llow e~ch te~m to visu~lize the CUR through Systems M~n~ger OpsCenter d~shbo~rds.

 Correct ;;nswer: B
 B (100%)

 Question #35
 ;; comp~ny is storing d~t~ on premises on ~ Windows  le server. The comp~ny produces 5 GB of new d~t~ d~ily. The comp~ny migr~ted p~rt of its Windows-b~sed worklo~d to ;;WS ~nd needs the d~t~ to be ~v~il~ble on ~  le system in the cloud. The comp~ny ~lre~dy h~s est~blished ~n ;;WS  Direct Connect connection between the on-premises network ~nd ;;WS. Which d~t~ migr~tion str~tegy should the comp~ny use?
  ;;. Use the  le g~tew~y option in ;;WS Stor~ge G~tew~y to repl~ce the existing Windows  le server, ~nd point the existing  le sh~re to the new  le g~tew~y.
  B. Use ;;WS  D~t~Sync to schedule ~ d~ily t~sk to replic~te d~t~ between the on-premises Windows  le server ~nd ;;m~zon  FSx.
  C. Use ;;WS  D~t~  Pipeline to schedule ~ d~ily t~sk to replic~te d~t~ between the on-premises Windows  le server ~nd ;;m~zon  El~stic  File System (;;m~zon  EFS).
  D. Use ;;WS  D~t~Sync to schedule ~ d~ily t~sk to replic~te d~t~ between the on-premises Windows  le server ~nd ;;m~zon  El~stic  File System (;;m~zon  EFS).

 Correct ;;nswer: B
 B (59%)                                  ;; (41%)

 Question #36
 ;; comp~ny’s solutions ~rchitect is reviewing ~ web ~pplic~tion th~t runs on ;;WS. The ~pplic~tion references st~tic ~ssets in ~n ;;m~zon S3 bucket in the us-e~st-1  Region. The comp~ny needs resiliency ~cross multiple ;;WS  Regions. The comp~ny ~lre~dy h~s cre~ted ~n S3 bucket in ~ second  Region. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Con gure the ~pplic~tion to write e~ch object to both S3 buckets. Set up ~n ;;m~zon  Route 53 public hosted zone with ~ record set by using ~ weighted routing policy for e~ch S3 bucket. Con gure the ~pplic~tion to reference the objects by using the  Route 53  DNS n~me.
  B. Cre~te ~n ;;WS  L~mbd~ function to copy objects from the S3 bucket in us-e~st-1 to the S3 bucket in the second  Region.  Invoke the  L~mbd~ function e~ch time ~n object is written to the S3 bucket in us-e~st-1. Set up ~n ;;m~zon CloudFront distribution with ~n origin group th~t cont~ins the two S3 buckets ~s origins.
  C. Con gure replic~tion on the S3 bucket in us-e~st-1 to replic~te objects to the S3 bucket in the second  Region. Set up ~n ;;m~zon CloudFront distribution with ~n origin group th~t cont~ins the two S3 buckets ~s origins.
  D. Con gure replic~tion on the S3 bucket in us-e~st-1 to replic~te objects to the S3 bucket in the second  Region.  If f~ilover is required, upd~te the ~pplic~tion code to lo~d S3 objects from the S3 bucket in the second  Region.

 Correct ;;nswer: D
 C (95%)                                    3%

 Question #37
 ;; comp~ny is hosting ~ three-tier web ~pplic~tion in ~n on-premises environment.  Due to ~ recent surge in tr~ c th~t resulted in downtime ~nd ~ signi c~nt  n~nci~l imp~ct, comp~ny m~n~gement h~s ordered th~t the ~pplic~tion be moved to ;;WS. The ~pplic~tion is written in .NET ~nd h~s ~ dependency on ~  MySQL d~t~b~se. ;; solutions ~rchitect must design ~ sc~l~ble ~nd highly ~v~il~ble solution to meet the dem~nd of 200,000 d~ily users. Which steps should the solutions ~rchitect t~ke to design ~n ~ppropri~te solution?
  ;;. Use ;;WS  El~stic  Be~nst~lk to cre~te ~ new ~pplic~tion with ~ web server environment ~nd ~n ;;m~zon  RDS  MySQL  Multi-;;Z  DB inst~nce. The environment should l~unch ~  Network  Lo~d  B~l~ncer (NLB) in front of ~n ;;m~zon  EC2 ;;uto Sc~ling group in multiple ;;v~il~bility Zones. Use ~n ;;m~zon  Route 53 ~li~s record to route tr~ c from the comp~ny’s dom~in to the  NLB.
  B. Use ;;WS CloudForm~tion to l~unch ~ st~ck cont~ining ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) in front of ~n ;;m~zon  EC2 ;;uto Sc~ling group sp~nning three ;;v~il~bility Zones. The st~ck should l~unch ~  Multi-;;Z deployment of ~n ;;m~zon ;;uror~  MySQL  DB cluster with ~  Ret~in deletion policy. Use ~n ;;m~zon  Route 53 ~li~s record to route tr~ c from the comp~ny’s dom~in to the ;;LB.
  C. Use ;;WS  El~stic  Be~nst~lk to cre~te ~n ~utom~tic~lly sc~ling web server environment th~t sp~ns two sep~r~te  Regions with ~n ;;pplic~tion Lo~d  B~l~ncer (;;LB) in e~ch  Region. Cre~te ~  Multi-;;Z deployment of ~n ;;m~zon ;;uror~  MySQL  DB cluster with ~ cross-Region re~d replic~. Use ;;m~zon  Route 53 with ~ geoproximity routing policy to route tr~ c between the two  Regions.
  D. Use ;;WS CloudForm~tion to l~unch ~ st~ck cont~ining ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) in front of ~n ;;m~zon  ECS cluster of Spot inst~nces sp~nning three ;;v~il~bility Zones. The st~ck should l~unch ~n ;;m~zon  RDS  MySQL  DB inst~nce with ~ Sn~pshot deletion policy. Use ~n ;;m~zon  Route 53 ~li~s record to route tr~ c from the comp~ny’s dom~in to the ;;LB.

 Correct ;;nswer: C
 B (93%)                                    4%

 Question #38
 ;; comp~ny is using ;;WS Org~niz~tions to m~n~ge multiple ;;WS ~ccounts.  For security purposes, the comp~ny requires the cre~tion of ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic th~t en~bles integr~tion with ~ third-p~rty ~lerting system in ~ll the Org~niz~tions member ~ccounts. ;; solutions ~rchitect used ~n ;;WS CloudForm~tion templ~te to cre~te the SNS topic ~nd st~ck sets to ~utom~te the deployment of CloudForm~tion st~cks. Trusted ~ccess h~s been en~bled in Org~niz~tions. Wh~t should the solutions ~rchitect do to deploy the CloudForm~tion St~ckSets in ~ll ;;WS ~ccounts?
  ;;. Cre~te ~ st~ck set in the Org~niz~tions member ~ccounts. Use service-m~n~ged permissions. Set deployment options to deploy to ~n org~niz~tion. Use CloudForm~tion St~ckSets drift detection.
  B. Cre~te st~cks in the Org~niz~tions member ~ccounts. Use self-service permissions. Set deployment options to deploy to ~n org~niz~tion. En~ble the CloudForm~tion St~ckSets ~utom~tic deployment.
  C. Cre~te ~ st~ck set in the Org~niz~tions m~n~gement ~ccount. Use service-m~n~ged permissions. Set deployment options to deploy to the org~niz~tion.  En~ble CloudForm~tion St~ckSets ~utom~tic deployment.
  D. Cre~te st~cks in the Org~niz~tions m~n~gement ~ccount. Use service-m~n~ged permissions. Set deployment options to deploy to the org~niz~tion.  En~ble CloudForm~tion St~ckSets drift detection.

 Correct ;;nswer: C  -
 C (100%)

 Question #39
 ;; comp~ny w~nts to migr~te its worklo~ds from on premises to ;;WS. The worklo~ds run on  Linux ~nd Windows. The comp~ny h~s ~ l~rge on- premises infr~structure th~t consists of physic~l m~chines ~nd VMs th~t host numerous ~pplic~tions. The comp~ny must c~pture det~ils ~bout the system con gur~tion, system perform~nce, running processes, ~nd network connections of its on- premises worklo~ds. The comp~ny ~lso must divide the on-premises ~pplic~tions into groups for ;;WS migr~tions. The comp~ny needs recommend~tions for ;;m~zon  EC2 inst~nce types so th~t the comp~ny c~n run its worklo~ds on ;;WS in the most cost-effective m~nner. Which combin~tion of steps should ~ solutions ~rchitect t~ke to meet these requirements? (Choose three.)
  ;;. ;;ssess the existing ~pplic~tions by inst~lling ;;WS ;;pplic~tion  Discovery ;;gent on the physic~l m~chines ~nd VMs.
  B. ;;ssess the existing ~pplic~tions by inst~lling ;;WS Systems  M~n~ger ;;gent on the physic~l m~chines ~nd VMs.
  C. Group servers into ~pplic~tions for migr~tion by using ;;WS Systems  M~n~ger ;;pplic~tion  M~n~ger.
  D. Group servers into ~pplic~tions for migr~tion by using ;;WS  Migr~tion  Hub.
  E. Gener~te recommended inst~nce types ~nd ~ssoci~ted costs by using ;;WS  Migr~tion  Hub.
  F.  Import d~t~ ~bout server sizes into ;;WS Trusted ;;dvisor.  Follow the recommend~tions for cost optimiz~tion.

 Correct ;;nswer: BDE
 ;;DE (93%)                                  7%

 Question #40
 ;; comp~ny is hosting ~n im~ge-processing service on ;;WS in ~ VPC. The VPC extends ~cross two ;;v~il~bility Zones.  E~ch ;;v~il~bility Zone cont~ins one public subnet ~nd one priv~te subnet. The service runs on ;;m~zon  EC2 inst~nces in the priv~te subnets. ;;n ;;pplic~tion  Lo~d  B~l~ncer in the public subnets is in front of the service. The service needs to communic~te with the internet ~nd does so through two  N;;T g~tew~ys. The service uses ;;m~zon S3 for im~ge stor~ge. The EC2 inst~nces retrieve ~pproxim~tely  1 ТВ of d~t~ from ~n S3 bucket e~ch d~y. The comp~ny h~s promoted the service ~s highly secure. ;; solutions ~rchitect must reduce cloud expenditures ~s much ~s possible without compromising the service’s security posture or incre~sing the time spent on ongoing oper~tions. Which solution will meet these requirements?
  ;;.  Repl~ce the  N;;T g~tew~ys with  N;;T inst~nces.  In the VPC route t~ble, cre~te ~ route from the priv~te subnets to the  N;;T inst~nces.
  B.  Move the  EC2 inst~nces to the public subnets.  Remove the  N;;T g~tew~ys.
  C. Set up ~n S3 g~tew~y VPC endpoint in the VP;;tt~ch ~n endpoint policy to the endpoint to ~llow the required ~ctions on the S3 bucket.
  D. ;;tt~ch ~n ;;m~zon  El~stic  File System (;;m~zon  EFS) volume to the  EC2 inst~nces.  Host the im~ges on the  EFS volume.

 Correct ;;nswer: C
 C (100%)

 Question #41
 ;; comp~ny recently deployed ~n ~pplic~tion on ;;WS. The ~pplic~tion uses ;;m~zon  Dyn~moDB. The comp~ny me~sured the ~pplic~tion lo~d ~nd con gured the  RCUs ~nd WCUs on the  Dyn~moDB t~ble to m~tch the expected pe~k lo~d. The pe~k lo~d occurs once ~ week for ~ 4-hour period ~nd is double the ~ver~ge lo~d. The ~pplic~tion lo~d is close to the ~ver~ge lo~d for the rest of the week. The ~ccess p~ttern includes m~ny more writes to the t~ble th~n re~ds of the t~ble. ;; solutions ~rchitect needs to implement ~ solution to minimize the cost of the t~ble. Which solution will meet these requirements?
  ;;. Use ;;WS ;;pplic~tion ;;uto Sc~ling to incre~se c~p~city during the pe~k period.  Purch~se reserved  RCUs ~nd WCUs to m~tch the ~ver~ge lo~d.
  B. Con gure on-dem~nd c~p~city mode for the t~ble.
  C. Con gure  Dyn~moDB ;;cceler~tor (D;;X) in front of the t~ble.  Reduce the provisioned re~d c~p~city to m~tch the new pe~k lo~d on the t~ble.
  D. Con gure  Dyn~moDB ;;cceler~tor (D;;X) in front of the t~ble. Con gure on-dem~nd c~p~city mode for the t~ble.

 Correct ;;nswer: D
 ;; (68%)                           B (17%)       14%

 Question #42
 ;; solutions ~rchitect needs to ~dvise ~ comp~ny on how to migr~te its on-premises d~t~ processing ~pplic~tion to the ;;WS Cloud. Currently, users uplo~d input  les through ~ web port~l. The web server then stores the uplo~ded  les on  N;;S ~nd mess~ges the processing server over ~ mess~ge queue.  E~ch medi~  le c~n t~ke up to  1 hour to process. The comp~ny h~s determined th~t the number of medi~  les ~w~iting processing is signi c~ntly higher during business hours, with the number of  les r~pidly declining ~fter business hours. Wh~t is the  MOST cost-effective migr~tion recommend~tion?
  ;;. Cre~te ~ queue using ;;m~zon SQS. Con gure the existing web server to publish to the new queue. When there ~re mess~ges in the queue, invoke ~n ;;WS  L~mbd~ function to pull requests from the queue ~nd process the  les. Store the processed  les in ~n ;;m~zon S3 bucket.
  B. Cre~te ~ queue using ;;m~zon  MQ. Con gure the existing web server to publish to the new queue. When there ~re mess~ges in the queue, cre~te ~ new ;;m~zon  EC2 inst~nce to pull requests from the queue ~nd process the  les. Store the processed  les in ;;m~zon  EFS. Shut down the  EC2 inst~nce ~fter the t~sk is complete.
  C. Cre~te ~ queue using ;;m~zon  MQ. Con gure the existing web server to publish to the new queue. When there ~re mess~ges in the queue, invoke ~n ;;WS  L~mbd~ function to pull requests from the queue ~nd process the  les. Store the processed  les in ;;m~zon  EFS.
  D. Cre~te ~ queue using ;;m~zon SQS. Con gure the existing web server to publish to the new queue. Use ;;m~zon  EC2 inst~nces in ~n  EC2 ;;uto Sc~ling group to pull requests from the queue ~nd process the  les. Sc~le the  EC2 inst~nces b~sed on the SQS queue length. Store the processed  les in ~n ;;m~zon S3 bucket.

 Correct ;;nswer: D
 D (95%)                                   2%

 Question #43
 ;; comp~ny is using ;;m~zon OpenSe~rch Service to ~n~lyze d~t~. The comp~ny lo~ds d~t~ into ~n OpenSe~rch Service cluster with  10 d~t~ nodes from ~n ;;m~zon S3 bucket th~t uses S3 St~nd~rd stor~ge. The d~t~ resides in the cluster for  1 month for re~d-only ~n~lysis. ;;fter  1 month, the comp~ny deletes the index th~t cont~ins the d~t~ from the cluster.  For compli~nce purposes, the comp~ny must ret~in ~ copy of ~ll input d~t~. The comp~ny is concerned ~bout ongoing costs ~nd ~sks ~ solutions ~rchitect to recommend ~ new solution. Which solution will meet these requirements  MOST cost-effectively?
  ;;.  Repl~ce ~ll the d~t~ nodes with Ultr~W~rm nodes to h~ndle the expected c~p~city. Tr~nsition the input d~t~ from S3 St~nd~rd to S3 Gl~cier Deep ;;rchive when the comp~ny lo~ds the d~t~ into the cluster.
  B.  Reduce the number of d~t~ nodes in the cluster to 2 ;;dd Ultr~W~rm nodes to h~ndle the expected c~p~city. Con gure the indexes to tr~nsition to Ultr~W~rm when OpenSe~rch Service ingests the d~t~. Tr~nsition the input d~t~ to S3 Gl~cier  Deep ;;rchive ~fter  1 month by using ~n S3  Lifecycle policy.
  C.  Reduce the number of d~t~ nodes in the cluster to 2. ;;dd Ultr~W~rm nodes to h~ndle the expected c~p~city. Con gure the indexes to tr~nsition to Ultr~W~rm when OpenSe~rch Service ingests the d~t~. ;;dd cold stor~ge nodes to the cluster Tr~nsition the indexes from Ultr~W~rm to cold stor~ge.  Delete the input d~t~ from the S3 bucket ~fter  1 month by using ~n S3  Lifecycle policy.
  D.  Reduce the number of d~t~ nodes in the cluster to 2. ;;dd inst~nce-b~cked d~t~ nodes to h~ndle the expected c~p~city. Tr~nsition the input d~t~ from S3 St~nd~rd to S3 Gl~cier  Deep ;;rchive when the comp~ny lo~ds the d~t~ into the cluster.

 Correct ;;nswer: B
 B (94%)                                   6%

 Question #44
 ;; comp~ny h~s  10 ~ccounts th~t ~re p~rt of ~n org~niz~tion in ;;WS Org~niz~tions. ;;WS Con g is con gured in e~ch ~ccount. ;;ll ~ccounts belong to either the  Prod OU or the  NonProd OU. The comp~ny h~s set up ~n ;;m~zon  EventBridge rule in e~ch ;;WS ~ccount to notify ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic when ~n ;;m~zon  EC2 security group inbound rule is cre~ted with 0.0.0.0/0 ~s the source. The comp~ny’s security te~m is subscribed to the SNS topic. For ~ll ~ccounts in the  NonProd OU, the security te~m needs to remove the ~bility to cre~te ~ security group inbound rule th~t includes 0.0.0.0/0 ~s the source. Which solution will meet this requirement with the  LE;;ST oper~tion~l overhe~d?
  ;;.  Modify the  EventBridge rule to invoke ~n ;;WS  L~mbd~ function to remove the security group inbound rule ~nd to publish to the SNS topic. Deploy the upd~ted rule to the  NonProd OU.
  B. ;;dd the vpc-sg-open-only-to-~uthorized-ports ;;WS Con g m~n~ged rule to the  NonProd OU.
  C. Con gure ~n SCP to ~llow the ec2:;;uthorizeSecurityGroupIngress ~ction when the v~lue of the ~ws:SourceIp condition key is not 0.0.0.0/0. ;;pply the SCP to the  NonProd OU.
  D. Con gure ~n SCP to deny the ec2:;;uthorizeSecurityGroupIngress ~ction when the v~lue of the ~ws:SourceIp condition key is 0.0.0.0/0. ;;pply the SCP to the  NonProd OU.

 Correct ;;nswer: C
 D (59%)                                ;; (38%)

 Question #45
 ;; comp~ny hosts ~ Git repository in ~n on-premises d~t~ center. The comp~ny uses webhooks to invoke function~lity th~t runs in the ;;WS Cloud. The comp~ny hosts the webhook logic on ~ set of ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group th~t the comp~ny set ~s ~ t~rget for ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The Git server c~lls the ;;LB for the con gured webhooks. The comp~ny w~nts to move the solution to ~ serverless ~rchitecture. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;.  For e~ch webhook, cre~te ~nd con gure ~n ;;WS  L~mbd~ function URL. Upd~te the Git servers to c~ll the individu~l  L~mbd~ function URLs.
  B. Cre~te ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI.  Implement e~ch webhook logic in ~ sep~r~te ;;WS  L~mbd~ function. Upd~te the Git servers to c~ll the ;;PI G~tew~y endpoint.
  C.  Deploy the webhook logic to ;;WS ;;pp  Runner. Cre~te ~n ;;LB, ~nd set ;;pp  Runner ~s the t~rget. Upd~te the Git servers to c~ll the ;;LB endpoint.
  D. Cont~inerize the webhook logic. Cre~te ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster, ~nd run the webhook logic in ;;WS F~rg~te. Cre~te ~n ;;m~zon ;;PI G~tew~y  REST ;;PI, ~nd set  F~rg~te ~s the t~rget. Upd~te the Git servers to c~ll the ;;PI G~tew~y endpoint.

 Correct ;;nswer: C
 B (81%)                                  Other

 Question #46
 ;; comp~ny is pl~nning to migr~te  1,000 on-premises servers to ;;WS. The servers run on sever~l VMw~re clusters in the comp~ny’s d~t~ center. ;;s p~rt of the migr~tion pl~n, the comp~ny w~nts to g~ther server metrics such ~s CPU det~ils,  R;;M us~ge, oper~ting system inform~tion, ~nd running processes. The comp~ny then w~nts to query ~nd ~n~lyze the d~t~. Which solution will meet these requirements?
  ;;.  Deploy ~nd con gure the ;;WS ;;gentless  Discovery Connector virtu~l ~ppli~nce on the on-premises hosts. Con gure  D~t~  Explor~tion in ;;WS  Migr~tion  Hub. Use ;;WS Glue to perform ~n  ETL job ~g~inst the d~t~. Query the d~t~ by using ;;m~zon S3 Select.
  B.  Export only the VM perform~nce inform~tion from the on-premises hosts.  Directly import the required d~t~ into ;;WS  Migr~tion  Hub. Upd~te ~ny missing inform~tion in  Migr~tion  Hub. Query the d~t~ by using ;;m~zon QuickSight.
  C. Cre~te ~ script to ~utom~tic~lly g~ther the server inform~tion from the on-premises hosts. Use the ;;WS CLI to run the put-resource- ~ttributes comm~nd to store the det~iled server d~t~ in ;;WS  Migr~tion  Hub. Query the d~t~ directly in the  Migr~tion  Hub console.
  D.  Deploy the ;;WS ;;pplic~tion  Discovery ;;gent to e~ch on-premises server. Con gure  D~t~  Explor~tion in ;;WS  Migr~tion  Hub. Use ;;m~zon ;;then~ to run prede ned queries ~g~inst the d~t~ in ;;m~zon S3.

 Correct ;;nswer: C
 D (91%)                                   9%

 Question #47
 ;; comp~ny is building ~ serverless ~pplic~tion th~t runs on ~n ;;WS  L~mbd~ function th~t is ~tt~ched to ~ VPC. The comp~ny needs to integr~te the ~pplic~tion with ~ new service from ~n extern~l provider. The extern~l provider supports only requests th~t come from public  IPv4 ~ddresses th~t ~re in ~n ~llow list. The comp~ny must provide ~ single public  IP ~ddress to the extern~l provider before the ~pplic~tion c~n st~rt using the new service. Which solution will give the ~pplic~tion the ~bility to ~ccess the new service?
  ;;.  Deploy ~  N;;T g~tew~y. ;;ssoci~te ~n  El~stic  IP ~ddress with the  N;;T g~tew~y. Con gure the VPC to use the  N;;T g~tew~y.
  B.  Deploy ~n egress-only internet g~tew~y. ;;ssoci~te ~n  El~stic  IP ~ddress with the egress-only internet g~tew~y. Con gure the el~stic network interf~ce on the  L~mbd~ function to use the egress-only internet g~tew~y.
  C.  Deploy ~n internet g~tew~y. ;;ssoci~te ~n  El~stic  IP ~ddress with the internet g~tew~y. Con gure the  L~mbd~ function to use the internet g~tew~y.
  D.  Deploy ~n internet g~tew~y. ;;ssoci~te ~n  El~stic  IP ~ddress with the internet g~tew~y. Con gure the def~ult route in the public VPC route t~ble to use the internet g~tew~y.

 Correct ;;nswer: C
 ;; (95%)                                    3%

 Question #48
 ;; solutions ~rchitect h~s developed ~ web ~pplic~tion th~t uses ~n ;;m~zon ;;PI G~tew~y  Region~l endpoint ~nd ~n ;;WS  L~mbd~ function. The consumers of the web ~pplic~tion ~re ~ll close to the ;;WS  Region where the ~pplic~tion will be deployed. The  L~mbd~ function only queries ~n ;;m~zon ;;uror~  MySQL d~t~b~se. The solutions ~rchitect h~s con gured the d~t~b~se to h~ve three re~d replic~s. During testing, the ~pplic~tion does not meet perform~nce requirements. Under high lo~d, the ~pplic~tion opens ~ l~rge number of d~t~b~se connections. The solutions ~rchitect must improve the ~pplic~tion’s perform~nce. Which ~ctions should the solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;. Use the cluster endpoint of the ;;uror~ d~t~b~se.
  B. Use  RDS  Proxy to set up ~ connection pool to the re~der endpoint of the ;;uror~ d~t~b~se.
  C. Use the  L~mbd~  Provisioned Concurrency fe~ture.
  D.  Move the code for opening the d~t~b~se connection in the  L~mbd~ function outside of the event h~ndler.
  E. Ch~nge the ;;PI G~tew~y endpoint to ~n edge-optimized endpoint.

 Correct ;;nswer: BD
 BD (98%)

 Question #49
 ;; comp~ny is pl~nning to host ~ web ~pplic~tion on ;;WS ~nd w~nts to lo~d b~l~nce the tr~ c ~cross ~ group of ;;m~zon  EC2 inst~nces. One of the security requirements is to en~ble end-to-end encryption in tr~nsit between the client ~nd the web server. Which solution will meet this requirement?
  ;;.  Pl~ce the  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB).  Provision ~n SSL certi c~te using ;;WS Certi c~te  M~n~ger (;;CM), ~nd ~ssoci~te the SSL certi c~te with the ;;LB.  Export the SSL certi c~te ~nd inst~ll it on e~ch  EC2 inst~nce. Con gure the ;;LB to listen on port 443 ~nd to forw~rd tr~ c to port 443 on the inst~nces.
  B. ;;ssoci~te the  EC2 inst~nces with ~ t~rget group.  Provision ~n SSL certi c~te using ;;WS Certi c~te  M~n~ger (;;CM). Cre~te ~n ;;m~zon CloudFront distribution ~nd con gure it to use the SSL certi c~te. Set CloudFront to use the t~rget group ~s the origin server.
  C.  Pl~ce the  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB)  Provision ~n SSL certi c~te using ;;WS Certi c~te  M~n~ger (;;CM), ~nd ~ssoci~te the SSL certi c~te with the ;;LB.  Provision ~ third-p~rty SSL certi c~te ~nd inst~ll it on e~ch  EC2 inst~nce. Con gure the ;;LB to listen on port 443 ~nd to forw~rd tr~ c to port 443 on the inst~nces.
  D.  Pl~ce the  EC2 inst~nces behind ~  Network  Lo~d  B~l~ncer (NLB).  Provision ~ third-p~rty SSL certi c~te ~nd inst~ll it on the  NLB ~nd on e~ch EC2 inst~nce. Con gure the  NLB to listen on port 443 ~nd to forw~rd tr~ c to port 443 on the inst~nces.

 Correct ;;nswer: C
 C (53%)                             D (35%)              11%

 Question #50
 ;; comp~ny w~nts to migr~te its d~t~ ~n~lytics environment from on premises to ;;WS. The environment consists of two simple  Node.js ~pplic~tions. One of the ~pplic~tions collects sensor d~t~ ~nd lo~ds it into ~  MySQL d~t~b~se. The other ~pplic~tion ~ggreg~tes the d~t~ into reports. When the ~ggreg~tion jobs run, some of the lo~d jobs f~il to run correctly. The comp~ny must resolve the d~t~ lo~ding issue. The comp~ny ~lso needs the migr~tion to occur without interruptions or ch~nges for the comp~ny’s customers. Wh~t should ~ solutions ~rchitect do to meet these requirements?
  ;;. Set up ~n ;;m~zon ;;uror~  MySQL d~t~b~se ~s ~ replic~tion t~rget for the on-premises d~t~b~se. Cre~te ~n ;;uror~  Replic~ for the ;;uror~ MySQL d~t~b~se, ~nd move the ~ggreg~tion jobs to run ~g~inst the ;;uror~  Replic~. Set up collection endpoints ~s ;;WS  L~mbd~ functions behind ~  Network  Lo~d  B~l~ncer (NLB), ~nd use ;;m~zon  RDS  Proxy to write to the ;;uror~  MySQL d~t~b~se. When the d~t~b~ses ~re synced, dis~ble the replic~tion job ~nd rest~rt the ;;uror~  Replic~ ~s the prim~ry inst~nce.  Point the collector  DNS record to the  NLB.
  B. Set up ~n ;;m~zon ;;uror~  MySQL d~t~b~se. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to perform continuous d~t~ replic~tion from the on-premises d~t~b~se to ;;uror~.  Move the ~ggreg~tion jobs to run ~g~inst the ;;uror~  MySQL d~t~b~se. Set up collection endpoints behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~s ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group. When the d~t~b~ses ~re synced, point the collector  DNS record to the ;;LDis~ble the ;;WS  DMS sync t~sk ~fter the cutover from on premises to ;;WS.
  C. Set up ~n ;;m~zon ;;uror~  MySQL d~t~b~se. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to perform continuous d~t~ replic~tion from the on-premises d~t~b~se to ;;uror~. Cre~te ~n ;;uror~  Replic~ for the ;;uror~  MySQL d~t~b~se, ~nd move the ~ggreg~tion jobs to run ~g~inst the ;;uror~  Replic~. Set up collection endpoints ~s ;;WS  L~mbd~ functions behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB), ~nd use ;;m~zon  RDS Proxy to write to the ;;uror~  MySQL d~t~b~se. When the d~t~b~ses ~re synced, point the collector  DNS record to the ;;LB.  Dis~ble the ;;WS DMS sync t~sk ~fter the cutover from on premises to ;;WS.
  D. Set up ~n ;;m~zon ;;uror~  MySQL d~t~b~se. Cre~te ~n ;;uror~  Replic~ for the ;;uror~  MySQL d~t~b~se, ~nd move the ~ggreg~tion jobs to run ~g~inst the ;;uror~  Replic~. Set up collection endpoints ~s ~n ;;m~zon  Kinesis d~t~ stre~m. Use ;;m~zon  Kinesis  D~t~  Firehose to replic~te the d~t~ to the ;;uror~  MySQL d~t~b~se. When the d~t~b~ses ~re synced, dis~ble the replic~tion job ~nd rest~rt the ;;uror~  Replic~ ~s the prim~ry inst~nce.  Point the collector  DNS record to the  Kinesis d~t~ stre~m.

 Correct ;;nswer: C
 C (95%)                                   5%

 Question #51
 ;; he~lth insur~nce comp~ny stores person~lly identi ~ble inform~tion (PII) in ~n ;;m~zon S3 bucket. The comp~ny uses server-side encryption with S3 m~n~ged encryption keys (SSE-S3) to encrypt the objects. ;;ccording to ~ new requirement, ~ll current ~nd future objects in the S3 bucket must be encrypted by keys th~t the comp~ny’s security te~m m~n~ges. The S3 bucket does not h~ve versioning en~bled. Which solution will meet these requirements?
  ;;.  In the S3 bucket properties, ch~nge the def~ult encryption to SSE-S3 with ~ customer m~n~ged key. Use the ;;WS CLI to re-uplo~d ~ll objects in the S3 bucket. Set ~n S3 bucket policy to deny unencrypted  PutObject requests.
  B.  In the S3 bucket properties, ch~nge the def~ult encryption to server-side encryption with ;;WS  KMS m~n~ged encryption keys (SSE-KMS). Set ~n S3 bucket policy to deny unencrypted  PutObject requests. Use the ;;WS CLI to re-uplo~d ~ll objects in the S3 bucket.
  C.  In the S3 bucket properties, ch~nge the def~ult encryption to server-side encryption with ;;WS  KMS m~n~ged encryption keys (SSE-KMS). Set ~n S3 bucket policy to ~utom~tic~lly encrypt objects on GetObject ~nd  PutObject requests.
  D.  In the S3 bucket properties, ch~nge the def~ult encryption to ;;ES-256 with ~ customer m~n~ged key. ;;tt~ch ~ policy to deny unencrypted PutObject requests to ~ny entities th~t ~ccess the S3 bucket. Use the ;;WS CLI to re-uplo~d ~ll objects in the S3 bucket.

 Correct ;;nswer: D
 B (59%)                                 D (41%)

 Question #52
 ;; comp~ny is running ~ web ~pplic~tion in the ;;WS Cloud. The ~pplic~tion consists of dyn~mic content th~t is cre~ted on ~ set of ;;m~zon  EC2 inst~nces. The  EC2 inst~nces run in ~n ;;uto Sc~ling group th~t is con gured ~s ~ t~rget group for ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The comp~ny is using ~n ;;m~zon CloudFront distribution to distribute the ~pplic~tion glob~lly. The CloudFront distribution uses the ;;LB ~s ~n origin. The comp~ny uses ;;m~zon  Route 53 for  DNS ~nd h~s cre~ted ~n ;; record of www.ex~mple.com for the CloudFront distribution. ;; solutions ~rchitect must con gure the ~pplic~tion so th~t itis highly ~v~il~ble ~nd f~ult toler~nt. Which solution meets these requirements?
  ;;.  Provision ~ full, second~ry ~pplic~tion deployment in ~ different ;;WS  Region. Upd~te the  Route 53 ;; record to be ~ f~ilover record. ;;dd both of the CloudFront distributions ~s v~lues. Cre~te  Route 53 he~lth checks.
  B.  Provision ~n ;;LB, ~n ;;uto Sc~ling group, ~nd  EC2 inst~nces in ~ different ;;WS  Region. Upd~te the CloudFront distribution, ~nd cre~te ~ second origin for the new ;;LCre~te ~n origin group for the two origins. Con gure one origin ~s prim~ry ~nd one origin ~s second~ry.
  C.  Provision ~n ;;uto Sc~ling group ~nd  EC2 inst~nces in ~ different ;;WS  Region. Cre~te ~ second t~rget for the new ;;uto Sc~ling group in the ;;LB. Set up the f~ilover routing ~lgorithm on the ;;LB.
  D.  Provision ~ full, second~ry ~pplic~tion deployment in ~ different ;;WS  Region. Cre~te ~ second CloudFront distribution, ~nd ~dd the new ~pplic~tion setup ~s ~n origin. Cre~te ~n ;;WS Glob~l ;;cceler~tor ~cceler~tor. ;;dd both of the CloudFront distributions ~s endpoints.

 Correct ;;nswer: B
 B (100%)

 Question #53
 ;; comp~ny h~s ~n org~niz~tion in ;;WS Org~niz~tions th~t h~s ~ l~rge number of ;;WS ~ccounts. One of the ;;WS ~ccounts is design~ted ~s ~ tr~nsit ~ccount ~nd h~s ~ tr~nsit g~tew~y th~t is sh~red with ~ll of the other ;;WS ~ccounts. ;;WS Site-to-Site VPN connections ~re con gured between ~ll of the comp~ny’s glob~l o ces ~nd the tr~nsit ~ccount. The comp~ny h~s ;;WS Con g en~bled on ~ll of its ~ccounts. The comp~ny’s networking te~m needs to centr~lly m~n~ge ~ list of intern~l  IP ~ddress r~nges th~t belong to the glob~l o ces.  Developers will reference this list to g~in ~ccess to their ~pplic~tions securely. Which solution meets these requirements with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;. Cre~te ~ JSON  le th~t is hosted in ;;m~zon S3 ~nd th~t lists ~ll of the intern~l  IP ~ddress r~nges. Con gure ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic in e~ch of the ~ccounts th~t c~n be invoked when the JSON  le is upd~ted. Subscribe ~n ;;WS  L~mbd~ function to the SNS topic to upd~te ~ll relev~nt security group rules with the upd~ted  IP ~ddress r~nges.
  B. Cre~te ~ new ;;WS Con g m~n~ged rule th~t cont~ins ~ll of the intern~l  IP ~ddress r~nges. Use the rule to check the security groups in e~ch of the ~ccounts to ensure compli~nce with the list of  IP ~ddress r~nges. Con gure the rule to ~utom~tic~lly remedi~te ~ny noncompli~nt security group th~t is detected.
  C.  In the tr~nsit ~ccount, cre~te ~ VPC pre x list with ~ll of the intern~l  IP ~ddress r~nges. Use ;;WS  Resource ;;ccess  M~n~ger to sh~re the pre x list with ~ll of the other ~ccounts. Use the sh~red pre x list to con gure security group rules in the other ~ccounts.
  D.  In the tr~nsit ~ccount, cre~te ~ security group with ~ll of the intern~l  IP ~ddress r~nges. Con gure the security groups in the other ~ccounts to reference the tr~nsit ~ccount’s security group by using ~ nested security group reference of “/sg-1~2b3c4d”.

 Correct ;;nswer: C
 C (100%)

 Question #54
 ;; comp~ny runs ~ new ~pplic~tion ~s ~ st~tic website in ;;m~zon S3. The comp~ny h~s deployed the ~pplic~tion to ~ production ;;WS ~ccount ~nd uses ;;m~zon CloudFront to deliver the website. The website c~lls ~n ;;m~zon ;;PI G~tew~y  REST ;;PI. ;;n ;;WS  L~mbd~ function b~cks e~ch ;;PI method. The comp~ny w~nts to cre~te ~ CSV report every 2 weeks to show e~ch ;;PI  L~mbd~ function’s recommended con gured memory, recommended cost, ~nd the price difference between current con gur~tions ~nd the recommend~tions. The comp~ny will store the reports in ~n S3 bucket. Which solution will meet these requirements with the  LE;;ST development time?
  ;;. Cre~te ~  L~mbd~ function th~t extr~cts metrics d~t~ for e~ch ;;PI  L~mbd~ function from ;;m~zon CloudW~tch  Logs for the 2-week period. Coll~te the d~t~ into t~bul~r form~t. Store the d~t~ ~s ~ .csv  le in ~n S3 bucket. Cre~te ~n ;;m~zon  EventBridge rule to schedule the  L~mbd~ function to run every 2 weeks.
  B. Opt in to ;;WS Compute Optimizer. Cre~te ~  L~mbd~ function th~t c~lls the  ExportL~mbd~FunctionRecommend~tions oper~tion.  Export the .csv  le to ~n S3 bucket. Cre~te ~n ;;m~zon  EventBridge rule to schedule the  L~mbd~ function to run every 2 weeks.
  C. Opt in to ;;WS Compute Optimizer. Set up enh~nced infr~structure metrics. Within the Compute Optimizer console, schedule ~ job to export the  L~mbd~ recommend~tions to ~ .csv  le. Store the  le in ~n S3 bucket every 2 weeks.
  D.  Purch~se the ;;WS  Business Support pl~n for the production ~ccount. Opt in to ;;WS Compute Optimizer for ;;WS Trusted ;;dvisor checks.  In the Trusted ;;dvisor console, schedule ~ job to export the cost optimiz~tion checks to ~ .csv  le. Store the  le in ~n S3 bucket every 2 weeks.

 Correct ;;nswer: B
 B (80%)                               D (15%)    5%

 Question #55
 ;; comp~ny’s f~ctory ~nd ~utom~tion ~pplic~tions ~re running in ~ single VPC.  More th~n 20 ~pplic~tions run on ~ combin~tion of ;;m~zon  EC2, ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS), ~nd ;;m~zon  RDS. The comp~ny h~s softw~re engineers spre~d ~cross three te~ms. One of the three te~ms owns e~ch ~pplic~tion, ~nd e~ch time is responsible for the cost ~nd perform~nce of ~ll of its ~pplic~tions. Te~m resources h~ve t~gs th~t represent their ~pplic~tion ~nd te~m. The te~ms use  I;;M ~ccess for d~ily ~ctivities. The comp~ny needs to determine which costs on the monthly ;;WS bill ~re ~ttribut~ble to e~ch ~pplic~tion or te~m. The comp~ny ~lso must be ~ble to cre~te reports to comp~re costs from the l~st  12 months ~nd to help forec~st costs for the next  12 months. ;; solutions ~rchitect must recommend ~n ;;WS  Billing ~nd Cost  M~n~gement solution th~t provides these cost reports. Which combin~tion of ~ctions will meet these requirements? (Choose three.)
  ;;. ;;ctiv~te the user-de ne cost ~lloc~tion t~gs th~t represent the ~pplic~tion ~nd the te~m.
  B. ;;ctiv~te the ;;WS gener~ted cost ~lloc~tion t~gs th~t represent the ~pplic~tion ~nd the te~m.
  C. Cre~te ~ cost c~tegory for e~ch ~pplic~tion in  Billing ~nd Cost  M~n~gement.
  D. ;;ctiv~te  I;;M ~ccess to  Billing ~nd Cost  M~n~gement.
  E. Cre~te ~ cost budget.
  F.  En~ble Cost  Explorer.

 Correct ;;nswer: ;;CF
 ;;CF (54%)                                ;;DF (46%)

 Question #56
 ;;n ;;WS customer h~s ~ web ~pplic~tion th~t runs on premises. The web ~pplic~tion fetches d~t~ from ~ third-p~rty ;;PI th~t is behind ~  rew~ll. The third p~rty ~ccepts only one public CIDR block in e~ch client’s ~llow list. The customer w~nts to migr~te their web ~pplic~tion to the ;;WS Cloud. The ~pplic~tion will be hosted on ~ set of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) in ~ VPC. The ;;LB is loc~ted in public subnets. The  EC2 inst~nces ~re loc~ted in priv~te subnets.  N;;T g~tew~ys provide internet ~ccess to the priv~te subnets. How should ~ solutions ~rchitect ensure th~t the web ~pplic~tion c~n continue to c~ll the third-p~rty ;;PI ~fter the migr~tion?
  ;;. ;;ssoci~te ~ block of customer-owned public  IP ~ddresses to the VPC.  En~ble public  IP ~ddressing for public subnets in the VPC.
  B.  Register ~ block of customer-owned public  IP ~ddresses in the ;;WS ~ccount. Cre~te  El~stic  IP ~ddresses from the ~ddress block ~nd ~ssign them to the  N;;T g~tew~ys in the VPC.
  C. Cre~te  El~stic  IP ~ddresses from the block of customer-owned  IP ~ddresses. ;;ssign the st~tic  El~stic  IP ~ddresses to the ;;LB.
  D.  Register ~ block of customer-owned public  IP ~ddresses in the ;;WS ~ccount. Set up ;;WS Glob~l ;;cceler~tor to use  El~stic  IP ~ddresses from the ~ddress block. Set the ;;LB ~s the ~cceler~tor endpoint.

 Correct ;;nswer: B
 B (100%)

 Question #57
 ;; comp~ny with sever~l ;;WS ~ccounts is using ;;WS Org~niz~tions ~nd service control policies (SCPs). ;;n ~dministr~tor cre~ted the following SCP ~nd h~s ~tt~ched it to ~n org~niz~tion~l unit (OU) th~t cont~ins ;;WS ~ccount  1111-1111-1111: Developers working in ~ccount  1111-1111-1111 compl~in th~t they c~nnot cre~te ;;m~zon S3 buckets.  How should the ~dministr~tor ~ddress this problem?
  ;;. ;;dd s3:Cre~teBucket with “;;llow” effect to the SCP.
  B.  Remove the ~ccount from the OU, ~nd ~tt~ch the SCP directly to ~ccount  1111-1111-1111.
  C.  Instruct the developers to ~dd ;;m~zon S3 permissions to their  I;;M entities.
  D.  Remove the SCP from ~ccount  1111-1111-1111.

 Correct ;;nswer: C
 C (87%)                                    13%

 Question #58
 ;; comp~ny h~s ~ monolithic ~pplic~tion th~t is critic~l to the comp~ny’s business. The comp~ny hosts the ~pplic~tion on ~n ;;m~zon  EC2 inst~nce th~t runs ;;m~zon  Linux 2. The comp~ny’s ~pplic~tion te~m receives ~ directive from the leg~l dep~rtment to b~ck up the d~t~ from the inst~nce’s encrypted ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume to ~n ;;m~zon S3 bucket. The ~pplic~tion te~m does not h~ve the ~dministr~tive SSH key p~ir for the inst~nce. The ~pplic~tion must continue to serve the users. Which solution will meet these requirements?
  ;;. ;;tt~ch ~ role to the inst~nce with permission to write to ;;m~zon S3. Use the ;;WS Systems  M~n~ger Session  M~n~ger option to g~in ~ccess to the inst~nce ~nd run comm~nds to copy d~t~ into ;;m~zon S3.
  B. Cre~te ~n im~ge of the inst~nce with the reboot option turned on.  L~unch ~ new  EC2 inst~nce from the im~ge. ;;tt~ch ~ role to the new inst~nce with permission to write to ;;m~zon S3.  Run ~ comm~nd to copy d~t~ into ;;m~zon S3.
  C. T~ke ~ sn~pshot of the  EBS volume by using ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM). Copy the d~t~ to ;;m~zon S3.
  D. Cre~te ~n im~ge of the inst~nce.  L~unch ~ new  EC2 inst~nce from the im~ge. ;;tt~ch ~ role to the new inst~nce with permission to write to ;;m~zon S3.  Run ~ comm~nd to copy d~t~ into ;;m~zon S3.

 Correct ;;nswer: ;;
 ;; (60%)                                 C (39%)

 Question #59
 ;; solutions ~rchitect needs to copy d~t~ from ~n ;;m~zon S3 bucket m ~n ;;WS ~ccount to ~ new S3 bucket in ~ new ;;WS ~ccount. The solutions ~rchitect must implement ~ solution th~t uses the ;;WS CLI. Which combin~tion of steps will successfully copy the d~t~? (Choose three.)
  ;;. Cre~te ~ bucket policy to ~llow the source bucket to list its contents ~nd to put objects ~nd set object ;;CLs in the destin~tion bucket. ;;tt~ch the bucket policy to the destin~tion bucket.
  B. Cre~te ~ bucket policy to ~llow ~ user in the destin~tion ~ccount to list the source bucket’s contents ~nd re~d the source bucket’s objects. ;;tt~ch the bucket policy to the source bucket.
  C. Cre~te ~n  I;;M policy in the source ~ccount. Con gure the policy to ~llow ~ user in the source ~ccount to list contents ~nd get objects in the source bucket, ~nd to list contents, put objects, ~nd set object ;;CLs in the destin~tion bucket. ;;tt~ch the policy to the user.
  D. Cre~te ~n  I;;M policy in the destin~tion ~ccount. Con gure the policy to ~llow ~ user in the destin~tion ~ccount to list contents ~nd get objects in the source bucket, ~nd to list contents, put objects, ~nd set object;;CLs in the destin~tion bucket. ;;tt~ch the policy to the user.
  E.  Run the ~ws s3 sync comm~nd ~s ~ user in the source ~ccount. Specify the source ~nd destin~tion buckets to copy the d~t~.
  F.  Run the ~ws s3 sync comm~nd ~s ~ user in the destin~tion ~ccount. Specify the source ~nd destin~tion buckets to copy the d~t~.

 Correct ;;nswer: ;;DF
 BDF (94%)                                    4%

 Question #60
 ;; comp~ny built ~n ~pplic~tion b~sed on ;;WS  L~mbd~ deployed in ~n ;;WS CloudForm~tion st~ck. The l~st production rele~se of the web ~pplic~tion introduced ~n issue th~t resulted in ~n out~ge l~sting sever~l minutes. ;; solutions ~rchitect must ~djust the deployment process to support ~ c~n~ry rele~se. Which solution will meet these requirements?
  ;;. Cre~te ~n ~li~s for every new deployed version of the  L~mbd~ function. Use the ;;WS CLI upd~te-~li~s comm~nd with the routing-con g p~r~meter to distribute the lo~d.
  B.  Deploy the ~pplic~tion into ~ new CloudForm~tion st~ck. Use ~n ;;m~zon  Route 53 weighted routing policy to distribute the lo~d.
  C. Cre~te ~ version for every new deployed  L~mbd~ function. Use the ;;WS CLI upd~te-function-con gur~tion comm~nd with the routing-con g p~r~meter to distribute the lo~d.
  D. Con gure ;;WS CodeDeploy ~nd use CodeDeployDef~ult.One;;t;;Time in the  Deployment con gur~tion to distribute the lo~d.

 Correct ;;nswer: ;;
 ;; (98%)

 Question #61
 ;;  n~nce comp~ny hosts ~ d~t~ l~ke in ;;m~zon S3. The comp~ny receives  n~nci~l d~t~ records over SFTP e~ch night from sever~l third p~rties. The comp~ny runs its own SFTP server on ~n ;;m~zon  EC2 inst~nce in ~ public subnet of ~ VPC. ;;fter the  les ~re uplo~ded, they ~re moved to the d~t~ l~ke by ~ cron job th~t runs on the s~me inst~nce. The SFTP server is re~ch~ble on  DNS sftp.ex~mple.com through the use of ;;m~zon  Route 53. Wh~t should ~ solutions ~rchitect do to improve the reli~bility ~nd sc~l~bility of the SFTP solution?
  ;;.  Move the  EC2 inst~nce into ~n ;;uto Sc~ling group.  Pl~ce the  EC2 inst~nce behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Upd~te the  DNS record sftp.ex~mple.com in  Route 53 to point to the ;;LB.
  B.  Migr~te the SFTP server to ;;WS Tr~nsfer for SFTP. Upd~te the  DNS record sftp.ex~mple.com in  Route 53 to point to the server endpoint hostn~me.
  C.  Migr~te the SFTP server to ~  le g~tew~y in ;;WS Stor~ge G~tew~y. Upd~te the  DNS record sftp.ex~mple.com in  Route 53 to point to the  le g~tew~y endpoint.
  D.  Pl~ce the  EC2 inst~nce behind ~  Network  Lo~d  B~l~ncer (NLB). Upd~te the  DNS record sftp.ex~mple.com in  Route 53 to point to the  NLB.

 Correct ;;nswer: B
 B (100%)

 Question #62
 ;; comp~ny w~nts to migr~te ~n ~pplic~tion to ;;m~zon  EC2 from VMw~re  Infr~structure th~t runs in ~n on-premises d~t~ center. ;; solutions ~rchitect must preserve the softw~re ~nd con gur~tion settings during the migr~tion. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Con gure the ;;WS  D~t~Sync ~gent to st~rt replic~ting the d~t~ store to ;;m~zon  FSx for Windows  File Server. Use the SMB sh~re to host the VMw~re d~t~ store. Use VM  Import/Export to move the VMs to ;;m~zon  EC2.
  B. Use the VMw~re vSphere client to export the ~pplic~tion ~s ~n im~ge in Open Virtu~liz~tion  Form~t (OVF) form~t. Cre~te ~n ;;m~zon S3 bucket to store the im~ge in the destin~tion ;;WS  Region. Cre~te ~nd ~pply ~n  I;;M role for VM  Import. Use the ;;WS CLI to run the  EC2 import comm~nd.
  C. Con gure ;;WS Stor~ge G~tew~y for  les service to export ~ Common  Internet  File System (CIFS) sh~re. Cre~te ~ b~ckup copy to the sh~red folder. Sign in to the ;;WS  M~n~gement Console ~nd cre~te ~n ;;MI from the b~ckup copy.  L~unch ~n  EC2 inst~nce th~t is b~sed on the ;;MI.
  D. Cre~te ~ m~n~ged-inst~nce ~ctiv~tion for ~ hybrid environment in ;;WS Systems  M~n~ger.  Downlo~d ~nd inst~ll Systems  M~n~ger ;;gent on the on-premises VM.  Register the VM with Systems  M~n~ger to be ~ m~n~ged inst~nce. Use ;;WS  B~ckup to cre~te ~ sn~pshot of the VM ~nd cre~te ~n ;;MI.  L~unch ~n  EC2 inst~nce th~t is b~sed on the ;;MI.

 Correct ;;nswer: D
 B (100%)

 Question #63
 ;; video processing comp~ny h~s ~n ~pplic~tion th~t downlo~ds im~ges from ~n ;;m~zon S3 bucket, processes the im~ges, stores ~ tr~nsformed im~ge in ~ second S3 bucket, ~nd upd~tes met~d~t~ ~bout the im~ge in ~n ;;m~zon  Dyn~moDB t~ble. The ~pplic~tion is written in  Node.js ~nd runs by using ~n ;;WS  L~mbd~ function. The  L~mbd~ function is invoked when ~ new im~ge is uplo~ded to ;;m~zon S3. The ~pplic~tion r~n without incident for ~ while.  However, the size of the im~ges h~s grown signi c~ntly. The  L~mbd~ function is now f~iling frequently with timeout errors. The function timeout is set to its m~ximum v~lue. ;; solutions ~rchitect needs to ref~ctor the ~pplic~tion’s ~rchitecture to prevent invoc~tion f~ilures. The comp~ny does not w~nt to m~n~ge the underlying infr~structure. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;.  Modify the ~pplic~tion deployment by building ~  Docker im~ge th~t cont~ins the ~pplic~tion code.  Publish the im~ge to ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR).
  B. Cre~te ~ new ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) t~sk de nition with ~ comp~tibility type of ;;WS  F~rg~te. Con gure the t~sk de nition to use the new im~ge in ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). ;;djust the  L~mbd~ function to invoke ~n  ECS t~sk by using the  ECS t~sk de nition when ~ new  le ~rrives in ;;m~zon S3.
  C. Cre~te ~n ;;WS Step  Functions st~te m~chine with ~  P~r~llel st~te to invoke the  L~mbd~ function.  Incre~se the provisioned concurrency of the  L~mbd~ function.
  D. Cre~te ~ new ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) t~sk de nition with ~ comp~tibility type of ;;m~zon  EC2. Con gure the t~sk de nition to use the new im~ge in ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). ;;djust the  L~mbd~ function to invoke ~n  ECS t~sk by using the  ECS t~sk de nition when ~ new  le ~rrives in ;;m~zon S3.
  E.  Modify the ~pplic~tion to store im~ges on ;;m~zon  El~stic  File System (;;m~zon  EFS) ~nd to store met~d~t~ on ~n ;;m~zon  RDS  DB inst~nce. ;;djust the  L~mbd~ function to mount the  EFS  le sh~re.

 Correct ;;nswer: DE
 ;;B (89%)                                   6%

 Question #64
 ;; comp~ny h~s ~n org~niz~tion in ;;WS Org~niz~tions. The comp~ny is using ;;WS Control Tower to deploy ~ l~nding zone for the org~niz~tion. The comp~ny w~nts to implement govern~nce ~nd policy enforcement. The comp~ny must implement ~ policy th~t will detect ;;m~zon  RDS  DB inst~nces th~t ~re not encrypted ~t rest in the comp~ny’s production OU. Which solution will meet this requirement?
  ;;. Turn on m~nd~tory gu~rdr~ils in ;;WS Control Tower. ;;pply the m~nd~tory gu~rdr~ils to the production OU.
  B.  En~ble the ~ppropri~te gu~rdr~il from the list of strongly recommended gu~rdr~ils in ;;WS Control Tower. ;;pply the gu~rdr~il to the production OU.
  C. Use ;;WS Con g to cre~te ~ new m~nd~tory gu~rdr~il. ;;pply the rule to ~ll ~ccounts in the production OU.
  D. Cre~te ~ custom SCP in ;;WS Control Tower. ;;pply the SCP to the production OU.

 Correct ;;nswer: B
 B (95%)                                    5%

 Question #65
 ;; st~rtup comp~ny hosts ~  eet of ;;m~zon  EC2 inst~nces in priv~te subnets using the l~test ;;m~zon  Linux 2 ;;MI. The comp~ny’s engineers rely he~vily on SSH ~ccess to the inst~nces for troubleshooting. The comp~ny’s existing ~rchitecture includes the following: • ;; VPC with priv~te ~nd public subnets, ~nd ~  N;;T g~tew~y. • Site-to-Site VPN for connectivity with the on-premises environment. •  EC2 security groups with direct SSH ~ccess from the on-premises environment. The comp~ny needs to incre~se security controls ~round SSH ~ccess ~nd provide ~uditing of comm~nds run by the engineers. Which str~tegy should ~ solutions ~rchitect use?
  ;;.  Inst~ll ~nd con gure  EC2  Inst~nce Connect on the  eet of  EC2 inst~nces.  Remove ~ll security group rules ~tt~ched to  EC2 inst~nces th~t ~llow inbound TCP on port 22. ;;dvise the engineers to remotely ~ccess the inst~nces by using the  EC2  Inst~nce Connect CLI.
  B. Upd~te the  EC2 security groups to only ~llow inbound TCP on port 22 to the  IP ~ddresses of the engineer’s devices.  Inst~ll the ;;m~zon CloudW~tch ~gent on ~ll  EC2 inst~nces ~nd send oper~ting system ~udit logs to CloudW~tch  Logs.
  C. Upd~te the  EC2 security groups to only ~llow inbound TCP on port 22 to the  IP ~ddresses of the engineer’s devices.  En~ble ;;WS Con g for EC2 security group resource ch~nges.  En~ble ;;WS  Firew~ll  M~n~ger ~nd ~pply ~ security group policy th~t ~utom~tic~lly remedi~tes ch~nges to rules.
  D. Cre~te ~n  I;;M role with the ;;m~zonSSMM~n~gedInst~nceCore m~n~ged policy ~tt~ched. ;;tt~ch the  I;;M role to ~ll the  EC2 inst~nces. Remove ~ll security group rules ~tt~ched to the  EC2 inst~nces th~t ~llow inbound TCP on port 22.  H~ve the engineers inst~ll the ;;WS Systems M~n~ger Session  M~n~ger plugin for their devices ~nd remotely ~ccess the inst~nces by using the st~rt-session ;;PI c~ll from Systems M~n~ger.

 Correct ;;nswer: D
 D (89%)                                  11%

 Question #66
 ;; comp~ny th~t uses ;;WS Org~niz~tions ~llows developers to experiment on ;;WS. ;;s p~rt of the l~nding zone th~t the comp~ny h~s deployed, developers use their comp~ny em~il ~ddress to request ~n ~ccount. The comp~ny w~nts to ensure th~t developers ~re not l~unching costly services or running services unnecess~rily. The comp~ny must give developers ~  xed monthly budget to limit their ;;WS costs. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Cre~te ~n SCP to set ~  xed monthly ~ccount us~ge limit. ;;pply the SCP to the developer ~ccounts.
  B. Use ;;WS  Budgets to cre~te ~  xed monthly budget for e~ch developer’s ~ccount ~s p~rt of the ~ccount cre~tion process.
  C. Cre~te ~n SCP to deny ~ccess to costly services ~nd components. ;;pply the SCP to the developer ~ccounts.
  D. Cre~te ~n  I;;M policy to deny ~ccess to costly services ~nd components. ;;pply the  I;;M policy to the developer ~ccounts.
  E. Cre~te ~n ;;WS  Budgets ~lert ~ction to termin~te services when the budgeted ~mount is re~ched. Con gure the ~ction to termin~te ~ll services.
  F. Cre~te ~n ;;WS  Budgets ~lert ~ction to send ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) noti c~tion when the budgeted ~mount is re~ched.  Invoke ~n ;;WS  L~mbd~ function to termin~te ~ll services.

 Correct ;;nswer: BDF
 BCF (76%)                                BDF (22%)

 Question #67
 ;; comp~ny h~s ~pplic~tions in ~n ;;WS ~ccount th~t is n~med Source. The ~ccount is in ~n org~niz~tion in ;;WS Org~niz~tions. One of the ~pplic~tions uses ;;WS  L~mbd~ functions ~nd stores inventory d~t~ in ~n ;;m~zon ;;uror~ d~t~b~se. The ~pplic~tion deploys the  L~mbd~ functions by using ~ deployment p~ck~ge. The comp~ny h~s con gured ~utom~ted b~ckups for ;;uror~. The comp~ny w~nts to migr~te the  L~mbd~ functions ~nd the ;;uror~ d~t~b~se to ~ new ;;WS ~ccount th~t is n~med T~rget. The ~pplic~tion processes critic~l d~t~, so the comp~ny must minimize downtime. Which solution will meet these requirements?
  ;;.  Downlo~d the  L~mbd~ function deployment p~ck~ge from the Source ~ccount. Use the deployment p~ck~ge ~nd cre~te new  L~mbd~ functions in the T~rget ~ccount. Sh~re the ~utom~ted ;;uror~  DB cluster sn~pshot with the T~rget ~ccount.
  B.  Downlo~d the  L~mbd~ function deployment p~ck~ge from the Source ~ccount. Use the deployment p~ck~ge ~nd cre~te new  L~mbd~ functions in the T~rget ~ccount. Sh~re the ;;uror~  DB cluster with the T~rget ~ccount by using ;;WS  Resource ;;ccess  M~n~ger {;;WS  R;;M). Gr~nt the T~rget ~ccount permission to clone the ;;uror~  DB cluster.
  C. Use ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M) to sh~re the  L~mbd~ functions ~nd the ;;uror~  DB cluster with the T~rget ~ccount. Gr~nt the T~rget ~ccount permission to clone the ;;uror~  DB cluster.
  D. Use ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M) to sh~re the  L~mbd~ functions with the T~rget ~ccount. Sh~re the ~utom~ted ;;uror~  DB cluster sn~pshot with the T~rget ~ccount.

 Correct ;;nswer: C
 B (98%)

 Question #68
 ;; comp~ny runs ~  Python script on ~n ;;m~zon  EC2 inst~nce to process d~t~. The script runs every  10 minutes. The script ingests  les from ~n ;;m~zon S3 bucket ~nd processes the  les. On ~ver~ge, the script t~kes ~pproxim~tely 5 minutes to process e~ch  le The script will not reprocess ~  le th~t the script h~s ~lre~dy processed. The comp~ny reviewed ;;m~zon CloudW~tch metrics ~nd noticed th~t the  EC2 inst~nce is idle for ~pproxim~tely 40% of the time bec~use of the  le processing speed. The comp~ny w~nts to m~ke the worklo~d highly ~v~il~ble ~nd sc~l~ble. The comp~ny ~lso w~nts to reduce long-term m~n~gement overhe~d. Which solution will meet these requirements  MOST cost-effectively?
  ;;.  Migr~te the d~t~ processing script to ~n ;;WS  L~mbd~ function. Use ~n S3 event noti c~tion to invoke the  L~mbd~ function to process the objects when the comp~ny uplo~ds the objects.
  B. Cre~te ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Con gure ;;m~zon S3 to send event noti c~tions to the SQS queue. Cre~te ~n  EC2 ;;uto Sc~ling group with ~ minimum size of one inst~nce. Upd~te the d~t~ processing script to poll the SQS queue.  Process the S3 objects th~t the SQS mess~ge identi es.
  C.  Migr~te the d~t~ processing script to ~ cont~iner im~ge.  Run the d~t~ processing cont~iner on ~n  EC2 inst~nce. Con gure the cont~iner to poll the S3 bucket for new objects ~nd to process the resulting objects.
  D.  Migr~te the d~t~ processing script to ~ cont~iner im~ge th~t runs on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ;;WS  F~rg~te. Cre~te ~n ;;WS  L~mbd~ function th~t c~lls the  F~rg~te  RunT~sk;;PI oper~tion when the cont~iner processes the  le. Use ~n S3 event noti c~tion to invoke the  L~mbd~ function.

 Correct ;;nswer: D
 ;; (76%)                                 D (24%)

 Question #69
 ;;  n~nci~l services comp~ny in  North ;;meric~ pl~ns to rele~se ~ new online web ~pplic~tion to its customers on ;;WS. The comp~ny will l~unch the ~pplic~tion in the us-e~st-1  Region on ;;m~zon  EC2 inst~nces. The ~pplic~tion must be highly ~v~il~ble ~nd must dyn~mic~lly sc~le to meet user tr~ c. The comp~ny ~lso w~nts to implement ~ dis~ster recovery environment for the ~pplic~tion in the us-west-1  Region by using ~ctive- p~ssive f~ilover. Which solution will meet these requirements?
  ;;. Cre~te ~ VPC in us-e~st-1 ~nd ~ VPC in us-west-1. Con gure VPC peering.  In the us-e~st-1 VPC, cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t extends ~cross multiple ;;v~il~bility Zones in both VPCs. Cre~te ~n ;;uto Sc~ling group th~t deploys the  EC2 inst~nces ~cross the multiple ;;v~il~bility Zones in both VPCs.  Pl~ce the ;;uto Sc~ling group behind the ;;LB.
  B. Cre~te ~ VPC in us-e~st-1 ~nd ~ VPC in us-west-1.  In the us-e~st-1 VPC, cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t extends ~cross multiple ;;v~il~bility Zones in th~t VPC. Cre~te ~n ;;uto Sc~ling group th~t deploys the  EC2 inst~nces ~cross the multiple ;;v~il~bility Zones in the us-e~st-1 VPC.  Pl~ce the ;;uto Sc~ling group behind the ;;LSet up the s~me con gur~tion in the us-west-1 VPC. Cre~te ~n ;;m~zon  Route 53 hosted zone. Cre~te sep~r~te records for e~ch ;;LEn~ble he~lth checks to ensure high ~v~il~bility between  Regions.
  C. Cre~te ~ VPC in us-e~st-1 ~nd ~ VPC in us-west-1.  In the us-e~st-1 VPC, cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t extends ~cross multiple ;;v~il~bility Zones in th~t VPCre~te ~n ;;uto Sc~ling group th~t deploys the  EC2 inst~nces ~cross the multiple ;;v~il~bility Zones in the us-e~st-1 VPPl~ce the ;;uto Sc~ling group behind the ;;LB. Set up the s~me con gur~tion in the us-west-1 VPCre~te ~n ;;m~zon  Route 53 hosted zone. Cre~te sep~r~te records for e~ch ;;LB.  En~ble he~lth checks ~nd con gure ~ f~ilover routing policy for e~ch record.
  D. Cre~te ~ VPC in us-e~st-1 ~nd ~ VPC in us-west-1. Con gure VPC peering.  In the us-e~st-1 VPC, cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t extends ~cross multiple ;;v~il~bility Zones in both VPCs. Cre~te ~n ;;uto Sc~ling group th~t deploys the  EC2 inst~nces ~cross the multiple ;;v~il~bility Zones in both VPCs.  Pl~ce the ;;uto Sc~ling group behind the ;;LB. Cre~te ~n ;;m~zon  Route 53 hosted zone. Cre~te ~ record for the ;;LB.

 Correct ;;nswer: C
 C (100%)

 Question #70
 ;; comp~ny h~s ~n environment th~t h~s ~ single ;;WS ~ccount. ;; solutions ~rchitect is reviewing the environment to recommend wh~t the comp~ny could improve speci c~lly in terms of ~ccess to the ;;WS  M~n~gement Console. The comp~ny’s  IT support workers currently ~ccess the console for ~dministr~tive t~sks, ~uthentic~ting with n~med  I;;M users th~t h~ve been m~pped to their job role. The  IT support workers no longer w~nt to m~int~in both their ;;ctive  Directory ~nd  I;;M user ~ccounts. They w~nt to be ~ble to ~ccess the console by using their existing ;;ctive  Directory credenti~ls. The solutions ~rchitect is using ;;WS  I;;M  Identity Center (;;WS Single Sign-On) to implement this function~lity. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Turn on the  I;;M  Identity Center fe~ture in Org~niz~tions. Cre~te ~nd con gure ~ directory in ;;WS  Directory Service for  Microsoft ;;ctive  Directory (;;WS  M~n~ged  Microsoft ;;D) with ~ two-w~y trust to the comp~ny’s on-premises ;;ctive Directory. Con gure  I;;M  Identity Center ~nd set the ;;WS  M~n~ged  Microsoft ;;D directory ~s the identity source. Cre~te permission sets ~nd m~p them to the existing groups within the ;;WS  M~n~ged  Microsoft ;;D directory.
  B. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Turn on the  I;;M  Identity Center fe~ture in Org~niz~tions. Cre~te ~nd con gure ~n ;;D Connector to connect to the comp~ny’s on-premises ;;ctive  Directory. Con gure  I;;M  Identity Center ~nd select the ;;D Connector ~s the identity source. Cre~te permission sets ~nd m~p them to the existing groups within the comp~ny’s ;;ctive  Directory.
  C. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Turn on ~ll fe~tures for the org~niz~tion. Cre~te ~nd con gure ~ directory in ;;WS  Directory Service for  Microsoft ;;ctive  Directory (;;WS  M~n~ged  Microsoft ;;D) with ~ two-w~y trust to the comp~ny’s on-premises ;;ctive  Directory. Con gure  I;;M  Identity Center ~nd select the ;;WS  M~n~ged  Microsoft ;;D directory ~s the identity source. Cre~te permission sets ~nd m~p them to the existing groups within the ;;WS  M~n~ged  Microsoft ;;D directory.
  D. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Turn on ~ll fe~tures for the org~niz~tion. Cre~te ~nd con gure ~n ;;D Connector to connect to the comp~ny’s on-premises ;;ctive  Directory. Con gure  I;;M  Identity Center ~nd set the ;;D Connector ~s the identity source. Cre~te permission sets ~nd m~p them to the existing groups within the comp~ny’s ;;ctive  Directory.

 Correct ;;nswer: D
 D (81%)                                   Other

 Question #71
 ;; video stre~ming comp~ny recently l~unched ~ mobile ~pp for video sh~ring. The ~pp uplo~ds v~rious  les to ~n ;;m~zon S3 bucket in the us- e~st-1  Region. The  les r~nge in size from  1 GB to  10 GB. Users who ~ccess the ~pp from ;;ustr~li~ h~ve experienced uplo~ds th~t t~ke long periods of time. Sometimes the  les f~il to completely uplo~d for these users. ;; solutions ~rchitect must improve the ~pp’s perform~nce for these uplo~ds. Which solutions will meet these requirements? (Choose two.)
  ;;.  En~ble S3 Tr~nsfer ;;cceler~tion on the S3 bucket. Con gure the ~pp to use the Tr~nsfer ;;cceler~tion endpoint for uplo~ds.
  B. Con gure ~n S3 bucket in e~ch  Region to receive the uplo~ds. Use S3 Cross-Region  Replic~tion to copy the  les to the distribution S3 bucket.
  C. Set up ;;m~zon  Route 53 with l~tency-b~sed routing to route the uplo~ds to the ne~rest S3 bucket  Region.
  D. Con gure the ~pp to bre~k the video  les into chunks. Use ~ multip~rt uplo~d to tr~nsfer  les to ;;m~zon S3.
  E.  Modify the ~pp to ~dd r~ndom pre xes to the  les before uplo~ding.

 Correct ;;nswer: ;;D
 ;;D (96%)                                    4%

 Question #72
 ;;n ~pplic~tion is using ~n ;;m~zon  RDS for  MySQL  Multi-;;Z  DB inst~nce in the us-e~st-1  Region. ;;fter ~ f~ilover test, the ~pplic~tion lost the connections to the d~t~b~se ~nd could not re-est~blish the connections. ;;fter ~ rest~rt of the ~pplic~tion, the ~pplic~tion re-est~blished the connections. ;; solutions ~rchitect must implement ~ solution so th~t the ~pplic~tion c~n re-est~blish connections to the d~t~b~se without requiring ~ rest~rt. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;m~zon ;;uror~  MySQL Serverless v1  DB inst~nce.  Migr~te the  RDS  DB inst~nce to the ;;uror~ Serverless v1  DB inst~nce. Upd~te the connection settings in the ~pplic~tion to point to the ;;uror~ re~der endpoint.
  B. Cre~te ~n  RDS proxy. Con gure the existing  RDS endpoint ~s ~ t~rget. Upd~te the connection settings in the ~pplic~tion to point to the  RDS proxy endpoint.
  C. Cre~te ~ two-node ;;m~zon ;;uror~  MySQL  DB cluster.  Migr~te the  RDS  DB inst~nce to the ;;uror~  DB cluster. Cre~te ~n  RDS proxy. Con gure the existing  RDS endpoint ~s ~ t~rget. Upd~te the connection settings in the ~pplic~tion to point to the  RDS proxy endpoint.
  D. Cre~te ~n ;;m~zon S3 bucket.  Export the d~t~b~se to ;;m~zon S3 by using ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS). Con gure ;;m~zon ;;then~ to use the S3 bucket ~s ~ d~t~ store.  Inst~ll the l~test Open  D~t~b~se Connectivity (ODBC) driver for the ~pplic~tion. Upd~te the connection settings in the ~pplic~tion to point to the ;;then~ endpoint

 Correct ;;nswer: B
 B (100%)

 Question #73
 ;; comp~ny is building ~ solution in the ;;WS Cloud. Thous~nds or devices will connect to the solution ~nd send d~t~.  E~ch device needs to be ~ble to send ~nd receive d~t~ in re~l time over the  MQTT protocol.  E~ch device must ~uthentic~te by using ~ unique X.509 certi c~te. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Set up ;;WS  IoT Core.  For e~ch device, cre~te ~ corresponding ;;m~zon  MQ queue ~nd provision ~ certi c~te. Connect e~ch device to ;;m~zon  MQ.
  B. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) ~nd con gure it with ~n ;;WS  L~mbd~ ~uthorizer.  Run ~n  MQTT broker on ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group. Set the ;;uto Sc~ling group ~s the t~rget for the  NLConnect e~ch device to the  NLB.
  C. Set up ;;WS  IoT Core.  For e~ch device, cre~te ~ corresponding ;;WS  IoT thing ~nd provision ~ certi c~te. Connect e~ch device to ;;WS  IoT Core.
  D. Set up ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI ~nd ~  Network  Lo~d  B~l~ncer (NLB). Cre~te integr~tion between ;;PI G~tew~y ~nd the  NLB. Con gure ~ mutu~l TLS certi c~te ~uthorizer on the  HTTP ;;PI.  Run ~n  MQTT broker on ~n ;;m~zon  EC2 inst~nce th~t the  NLB t~rgets. Connect e~ch device to the  NLB.

 Correct ;;nswer: D
 C (95%)                                    5%

 Question #74
 ;; comp~ny is running sever~l worklo~ds in ~ single ;;WS ~ccount. ;; new comp~ny policy st~tes th~t engineers c~n provision only ~pproved resources ~nd th~t engineers must use ;;WS CloudForm~tion to provision these resources. ;; solutions ~rchitect needs to cre~te ~ solution to enforce the new restriction on the  I;;M role th~t the engineers use for ~ccess. Wh~t should the solutions ~rchitect do to cre~te the solution?
  ;;. Uplo~d ;;WS CloudForm~tion templ~tes th~t cont~in ~pproved resources to ~n ;;m~zon S3 bucket. Upd~te the  I;;M policy for the engineers’ I;;M role to only ~llow ~ccess to ;;m~zon S3 ~nd ;;WS CloudForm~tion. Use ;;WS CloudForm~tion templ~tes to provision resources.
  B. Upd~te the  I;;M policy for the engineers’  I;;M role with permissions to only ~llow provisioning of ~pproved resources ~nd ;;WS CloudForm~tion. Use ;;WS CloudForm~tion templ~tes to cre~te st~cks with ~pproved resources.
  C. Upd~te the  I;;M policy for the engineers’  I;;M role with permissions to only ~llow ;;WS CloudForm~tion ~ctions. Cre~te ~ new  I;;M policy with permission to provision ~pproved resources, ~nd ~ssign the policy to ~ new  I;;M service role. ;;ssign the  I;;M service role to ;;WS CloudForm~tion during st~ck cre~tion.
  D.  Provision resources in ;;WS CloudForm~tion st~cks. Upd~te the  I;;M policy for the engineers’  I;;M role to only ~llow ~ccess to their own ;;WS CloudForm~tion st~ck.

 Correct ;;nswer: B
 C (98%)

 Question #75
 ;; solutions ~rchitect is designing the d~t~ stor~ge ~nd retriev~l ~rchitecture for ~ new ~pplic~tion th~t ~ comp~ny will be l~unching soon. The ~pplic~tion is designed to ingest millions of sm~ll records per minute from devices ~ll ~round the world.  E~ch record is less th~n 4  KB in size ~nd needs to be stored in ~ dur~ble loc~tion where it c~n be retrieved with low l~tency. The d~t~ is ephemer~l ~nd the comp~ny is required to store the d~t~ for  120 d~ys only, ~fter which the d~t~ c~n be deleted. The solutions ~rchitect c~lcul~tes th~t, during the course of ~ ye~r, the stor~ge requirements would be ~bout  10-15 TB. Which stor~ge str~tegy is the  MOST cost-effective ~nd meets the design requirements?
  ;;.  Design the ~pplic~tion to store e~ch incoming record ~s ~ single .csv  le in ~n ;;m~zon S3 bucket to ~llow for indexed retriev~l. Con gure ~ lifecycle policy to delete d~t~ older th~n  120 d~ys.
  B.  Design the ~pplic~tion to store e~ch incoming record in ~n ;;m~zon  Dyn~moDB t~ble properly con gured for the sc~le. Con gure the Dyn~moDB Time to  Live (TTL) fe~ture to delete records older th~n  120 d~ys.
  C.  Design the ~pplic~tion to store e~ch incoming record in ~ single t~ble in ~n ;;m~zon  RDS  MySQL d~t~b~se.  Run ~ nightly cron job th~t runs ~ query to delete ~ny records older th~n  120 d~ys.
  D.  Design the ~pplic~tion to b~tch incoming records before writing them to ~n ;;m~zon S3 bucket. Upd~te the met~d~t~ for the object to cont~in the list of records in the b~tch ~nd use the ;;m~zon S3 met~d~t~ se~rch fe~ture to retrieve the d~t~. Con gure ~ lifecycle policy to delete the d~t~ ~fter  120 d~ys.

 Correct ;;nswer: B
 B (78%)                                  D (22%)

 Question #76
 ;; ret~il comp~ny is hosting ~n ecommerce website on ;;WS ~cross multiple ;;WS  Regions. The comp~ny w~nts the website to be oper~tion~l ~t ~ll times for online purch~ses. The website stores d~t~ in ~n ;;m~zon  RDS for  MySQL  DB inst~nce. Which solution will provide the  HIGHEST ~v~il~bility for the d~t~b~se?
  ;;. Con gure ~utom~ted b~ckups on ;;m~zon  RDS.  In the c~se of disruption, promote ~n ~utom~ted b~ckup to be ~ st~nd~lone  DB inst~nce. Direct d~t~b~se tr~ c to the promoted  DB inst~nce. Cre~te ~ repl~cement re~d replic~ th~t h~s the promoted  DB inst~nce ~s its source.
  B. Con gure glob~l t~bles ~nd re~d replic~s on ;;m~zon  RDS. ;;ctiv~te the cross-Region scope.  In the c~se of disruption, use ;;WS  L~mbd~ to copy the re~d replic~s from one  Region to ~nother  Region.
  C. Con gure glob~l t~bles ~nd ~utom~ted b~ckups on ;;m~zon  RDS.  In the c~se of disruption, use ;;WS  L~mbd~ to copy the re~d replic~s from one  Region to ~nother  Region.
  D. Con gure re~d replic~s on ;;m~zon  RDS.  In the c~se of disruption, promote ~ cross-Region ~nd re~d replic~ to be ~ st~nd~lone  DB inst~nce. Direct d~t~b~se tr~ c to the promoted  DB inst~nce. Cre~te ~ repl~cement re~d replic~ th~t h~s the promoted  DB inst~nce ~s its source.

 Correct ;;nswer: D
 D (92%)                                    8%

 Question #77
 Ex~mple Corp. h~s ~n on-premises d~t~ center ~nd ~ VPC n~med VPC ;; in the  Ex~mple Corp. ;;WS ~ccount. The on-premises network connects to VPC ;; through ~n ;;WS Site-To-Site VPN. The on-premises servers c~n properly ~ccess VPC ;;.  Ex~mple Corp. just ~cquired ;;nyComp~ny, which h~s ~ VPC n~med VPC  B. There is no  IP ~ddress overl~p ~mong these networks.  Ex~mple Corp. h~s peered VPC ;; ~nd VPC  B. Ex~mple Corp. w~nts to connect from its on-premise servers to VPC  B.  Ex~mple Corp. h~s properly set up the network ;;CL ~nd security groups. Which solution will meet this requirement with the  LE;;ST oper~tion~l effort?
  ;;. Cre~te ~ tr~nsit g~tew~y. ;;tt~ch the Site-to-Site VPN, VPC ;;, ~nd VPC  B to the tr~nsit g~tew~y. Upd~te the tr~nsit g~tew~y route t~bles for ~ll networks to ~dd  IP r~nge routes for ~ll other networks.
  B. Cre~te ~ tr~nsit g~tew~y. Cre~te ~ Site-to-Site VPN connection between the on-premises network ~nd VPC  B, ~nd connect the VPN connection to the tr~nsit g~tew~y. ;;dd ~ route to direct tr~ c to the peered VPCs, ~nd ~dd ~n ~uthoriz~tion rule to give clients ~ccess to the VPCs ;; ~nd  B.
  C. Upd~te the route t~bles for the Site-to-Site VPN ~nd both VPCs for ~ll three networks. Con gure  BGP prop~g~tion for ~ll three networks. W~it for up to 5 minutes for  BGP prop~g~tion to  nish.
  D.  Modify the Site-to-Site VPN’s virtu~l priv~te g~tew~y de nition to include VPC ;; ~nd VPC  B. Split the two routers of the virtu~l priv~te get~w~y between the two VPCs.

 Correct ;;nswer: D
 ;; (88%)                                    8%

 Question #78
 ;; comp~ny recently completed the migr~tion from ~n on-premises d~t~ center to the ;;WS Cloud by using ~ repl~tforming str~tegy. One of the migr~ted servers is running ~ leg~cy Simple  M~il Tr~nsfer  Protocol (SMTP) service th~t ~ critic~l ~pplic~tion relies upon. The ~pplic~tion sends outbound em~il mess~ges to the comp~ny’s customers. The leg~cy SMTP server does not support TLS encryption ~nd uses TCP port 25. The ~pplic~tion c~n use SMTP only. The comp~ny decides to use ;;m~zon Simple  Em~il Service (;;m~zon SES) ~nd to decommission the leg~cy SMTP server. The comp~ny h~s cre~ted ~nd v~lid~ted the SES dom~in. The comp~ny h~s lifted the SES limits. Wh~t should the comp~ny do to modify the ~pplic~tion to send em~il mess~ges from ;;m~zon SES?
  ;;. Con gure the ~pplic~tion to connect to ;;m~zon SES by using TLS Wr~pper. Cre~te ~n  I;;M role th~t h~s ses:SendEm~il ~nd ses:SendR~wEm~il permissions. ;;tt~ch the  I;;M role to ~n ;;m~zon  EC2 inst~nce.
  B. Con gure the ~pplic~tion to connect to ;;m~zon SES by using ST;;RTTLS. Obt~in ;;m~zon SES SMTP credenti~ls. Use the credenti~ls to ~uthentic~te with ;;m~zon SES.
  C. Con gure the ~pplic~tion to use the SES ;;PI to send em~il mess~ges. Cre~te ~n  I;;M role th~t h~s ses:SendEm~il ~nd ses:SendR~wEm~il permissions. Use the  I;;M role ~s ~ service role for ;;m~zon SES.
  D. Con gure the ~pplic~tion to use ;;WS SDKs to send em~il mess~ges. Cre~te ~n  I;;M user for ;;m~zon SES. Gener~te ;;PI ~ccess keys. Use the ~ccess keys to ~uthentic~te with ;;m~zon SES.

 Correct ;;nswer: ;;
 B (86%)                                   12%

 Question #79
 ;; comp~ny recently ~cquired sever~l other comp~nies.  E~ch comp~ny h~s ~ sep~r~te ;;WS ~ccount with ~ different billing ~nd reporting method. The ~cquiring comp~ny h~s consolid~ted ~ll the ~ccounts into one org~niz~tion in ;;WS Org~niz~tions.  However, the ~cquiring comp~ny h~s found it di cult to gener~te ~ cost report th~t cont~ins me~ningful groups for ~ll the te~ms. The ~cquiring comp~ny’s  n~nce te~m needs ~ solution to report on costs for ~ll the comp~nies through ~ self-m~n~ged ~pplic~tion. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;WS Cost ~nd Us~ge  Report for the org~niz~tion.  De ne t~gs ~nd cost c~tegories in the report. Cre~te ~ t~ble in ;;m~zon ;;then~. Cre~te ~n ;;m~zon QuickSight d~t~set b~sed on the ;;then~ t~ble. Sh~re the d~t~set with the  n~nce te~m.
  B. Cre~te ~n ;;WS Cost ~nd Us~ge  Report for the org~niz~tion.  De ne t~gs ~nd cost c~tegories in the report. Cre~te ~ speci~lized templ~te in ;;WS Cost  Explorer th~t the  n~nce dep~rtment will use to build reports.
  C. Cre~te ~n ;;m~zon QuickSight d~t~set th~t receives spending inform~tion from the ;;WS  Price  List Query ;;PI. Sh~re the d~t~set with the  n~nce te~m.
  D. Use the ;;WS  Price  List Query ;;PI to collect ~ccount spending inform~tion. Cre~te ~ speci~lized templ~te in ;;WS Cost  Explorer th~t the  n~nce dep~rtment will use to build reports.

 Correct ;;nswer: D
 ;; (100%)

 Question #80
 ;; comp~ny runs ~n  IoT pl~tform on ;;WS.  IoT sensors in v~rious loc~tions send d~t~ to the comp~ny’s  Node.js ;;PI servers on ;;m~zon  EC2 inst~nces running behind ~n ;;pplic~tion  Lo~d  B~l~ncer. The d~t~ is stored in ~n ;;m~zon  RDS  MySQL  DB inst~nce th~t uses ~ 4 TB Gener~l Purpose SSD volume. The number of sensors the comp~ny h~s deployed in the  eld h~s incre~sed over time, ~nd is expected to grow signi c~ntly. The ;;PI servers ~re consistently overlo~ded ~nd  RDS metrics show high write l~tency. Which of the following steps together will resolve the issues perm~nently ~nd en~ble growth ~s new sensors ~re provisioned, while keeping this pl~tform cost-e cient? (Choose two.)
  ;;.  Resize the  MySQL Gener~l  Purpose SSD stor~ge to 6 TB to improve the volume’s  IOPS.
  B.  Re-~rchitect the d~t~b~se tier to use ;;m~zon ;;uror~ inste~d of ~n  RDS  MySQL  DB inst~nce ~nd ~dd re~d replic~s.
  C.  Lever~ge ;;m~zon  Kinesis  D~t~ Stre~ms ~nd ;;WS  L~mbd~ to ingest ~nd process the r~w d~t~.
  D. Use ;;WS X-R~y to ~n~lyze ~nd debug ~pplic~tion issues ~nd ~dd more ;;PI servers to m~tch the lo~d.
  E.  Re-~rchitect the d~t~b~se tier to use ;;m~zon  Dyn~moDB inste~d of ~n  RDS  MySQL  DB inst~nce.

 Correct ;;nswer: CE
 CE (66%)                          BC (17%)       Other

 Question #81
 ;; comp~ny is building ~n electronic document m~n~gement system in which users uplo~d their documents. The ~pplic~tion st~ck is entirely serverless ~nd runs on ;;WS in the eu-centr~l-1  Region. The system includes ~ web ~pplic~tion th~t uses ~n ;;m~zon CloudFront distribution for delivery with ;;m~zon S3 ~s the origin. The web ~pplic~tion communic~tes with ;;m~zon ;;PI G~tew~y  Region~l endpoints. The ;;PI G~tew~y ;;PIs c~ll ;;WS  L~mbd~ functions th~t store met~d~t~ in ~n ;;m~zon ;;uror~ Serverless d~t~b~se ~nd put the documents into ~n S3 bucket. The comp~ny is growing ste~dily ~nd h~s completed ~ proof of concept with its l~rgest customer. The comp~ny must improve l~tency outside of Europe. Which combin~tion of ~ctions will meet these requirements? (Choose two.)
  ;;.  En~ble S3 Tr~nsfer ;;cceler~tion on the S3 bucket.  Ensure th~t the web ~pplic~tion uses the Tr~nsfer ;;cceler~tion signed URLs.
  B. Cre~te ~n ~cceler~tor in ;;WS Glob~l ;;cceler~tor. ;;tt~ch the ~cceler~tor to the CloudFront distribution.
  C. Ch~nge the ;;PI G~tew~y  Region~l endpoints to edge-optimized endpoints.
  D.  Provision the entire st~ck in two other loc~tions th~t ~re spre~d ~cross the world. Use glob~l d~t~b~ses on the ;;uror~ Serverless cluster.
  E. ;;dd ~n ;;m~zon  RDS proxy between the  L~mbd~ functions ~nd the ;;uror~ Serverless d~t~b~se.

 Correct ;;nswer: ;;C
 ;;C (51%)                           CD (36%)               8%

 Question #82
 ;;n ~dventure comp~ny h~s l~unched ~ new fe~ture on its mobile ~pp. Users c~n use the fe~ture to uplo~d their hiking ~nd r~fting photos ~nd videos ~nytime. The photos ~nd videos ~re stored in ;;m~zon S3 St~nd~rd stor~ge in ~n S3 bucket ~nd ~re served through ;;m~zon CloudFront. The comp~ny needs to optimize the cost of the stor~ge. ;; solutions ~rchitect discovers th~t most of the uplo~ded photos ~nd videos ~re ~ccessed infrequently ~fter 30 d~ys.  However, some of the uplo~ded photos ~nd videos ~re ~ccessed frequently ~fter 30 d~ys. The solutions ~rchitect needs to implement ~ solution th~t m~int~ins millisecond retriev~l ~v~il~bility of the photos ~nd videos ~t the lowest possible cost. Which solution will meet these requirements?
  ;;. Con gure S3  Intelligent-Tiering on the S3 bucket.
  B. Con gure ~n S3  Lifecycle policy to tr~nsition im~ge objects ~nd video objects from S3 St~nd~rd to S3 Gl~cier  Deep ;;rchive ~fter 30 d~ys.
  C.  Repl~ce ;;m~zon S3 with ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system th~t is mounted on ;;m~zon  EC2 inst~nces.
  D. ;;dd ~ C~che-Control: m~x-~ge he~der to the S3 im~ge objects ~nd S3 video objects. Set the he~der to 30 d~ys.

 Correct ;;nswer: B
 ;; (96%)                                    4%

 Question #83
 ;; comp~ny uses ;;m~zon S3 to store  les ~nd im~ges in ~ v~riety of stor~ge cl~sses. The comp~ny's S3 costs h~ve incre~sed subst~nti~lly during the p~st ye~r. ;; solutions ~rchitect needs to review d~t~ trends for the p~st  12 months ~nd identity the ~ppropri~te stor~ge cl~ss for the objects. Which solution will meet these requirements?
  ;;.  Downlo~d ;;WS Cost ~nd Us~ge  Reports for the l~st  12 months of S3 us~ge.  Review ;;WS Trusted ;;dvisor recommend~tions for cost s~vings.
  B. Use S3 stor~ge cl~ss ~n~lysis.  Import d~t~ trends into ~n ;;m~zon QuickSight d~shbo~rd to ~n~lyze stor~ge trends.
  C. Use ;;m~zon S3 Stor~ge  Lens. Upgr~de the def~ult d~shbo~rd to include ~dv~nced metrics for stor~ge trends.
  D. Use ;;ccess ;;n~lyzer for S3.  Downlo~d the ;;ccess ;;n~lyzer for S3 report for the l~st  12 months.  Import the .csv  le to ~n ;;m~zon QuickSight d~shbo~rd.

 Correct ;;nswer: B
 C (76%)                                14%       10%

 Question #84
 ;; comp~ny h~s its cloud infr~structure on ;;WS. ;; solutions ~rchitect needs to de ne the infr~structure ~s code. The infr~structure is currently deployed in one ;;WS  Region. The comp~ny’s business exp~nsion pl~n includes deployments in multiple  Regions ~cross multiple ;;WS ~ccounts. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Use ;;WS CloudForm~tion templ~tes. ;;dd  I;;M policies to control the v~rious ~ccounts,  Deploy the templ~tes ~cross the multiple  Regions.
  B. Use ;;WS Org~niz~tions.  Deploy ;;WS CloudForm~tion templ~tes from the m~n~gement ~ccount Use ;;WS Control Tower to m~n~ge deployments ~cross ~ccounts.
  C. Use ;;WS Org~niz~tions ~nd ;;WS CloudForm~tion St~ckSets.  Deploy ~ Cloud  Form~tion templ~te from ~n ~ccount th~t h~s the necess~ry I;;M permissions.
  D. Use nested st~cks with ;;WS CloudForm~tion templ~tes. Ch~nge the  Region by using nested st~cks.

 Correct ;;nswer: C
 C (100%)

 Question #85
 ;; comp~ny h~s its cloud infr~structure on ;;WS. ;; solutions ~rchitect needs to de ne the infr~structure ~s code. The infr~structure is currently deployed in one ;;WS  Region. The comp~ny’s business exp~nsion pl~n includes deployments in multiple  Regions ~cross multiple ;;WS ~ccounts. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Use ;;WS CloudForm~tion templ~tes. ;;dd  I;;M policies to control the v~rious ~ccounts,  Deploy the templ~tes ~cross the multiple  Regions.
  B. Use ;;WS Org~niz~tions.  Deploy ;;WS CloudForm~tion templ~tes from the m~n~gement ~ccount Use ;;WS Control Tower to m~n~ge deployments ~cross ~ccounts.
  C. Use ;;WS Org~niz~tions ~nd ;;WS CloudForm~tion St~ckSets.  Deploy ~ Cloud  Form~tion templ~te from ~n ~ccount th~t h~s the necess~ry I;;M permissions.
  D. Use nested st~cks with ;;WS CloudForm~tion templ~tes. Ch~nge the  Region by using nested st~cks.

 Correct ;;nswer: C
 C (100%)

 Question #86
 ;; comp~ny pl~ns to ref~ctor ~ monolithic ~pplic~tion into ~ modern ~pplic~tion design deployed on ;;WS. The CI/CD pipeline needs to be upgr~ded to support the modern design for the ~pplic~tion with the following requirements: •  It should ~llow ch~nges to be rele~sed sever~l times every hour. •  It should be ~ble to roll b~ck the ch~nges ~s quickly ~s possible. Which design will meet these requirements?
  ;;.  Deploy ~ CI/CD pipeline th~t incorpor~tes ;;MIs to cont~in the ~pplic~tion ~nd their con gur~tions.  Deploy the ~pplic~tion by repl~cing ;;m~zon  EC2 inst~nces.
  B. Specify ;;WS  El~stic  Be~nst~lk to st~ge in ~ second~ry environment ~s the deployment t~rget for the CI/CD pipeline of the ~pplic~tion. To deploy, sw~p the st~ging ~nd production environment URLs.
  C. Use ;;WS Systems  M~n~ger to re-provision the infr~structure for e~ch deployment. Upd~te the ;;m~zon  EC2 user d~t~ to pull the l~test code ~rtif~ct from ;;m~zon S3 ~nd use ;;m~zon  Route 53 weighted routing to point to the new environment.
  D.  Roll out the ~pplic~tion upd~tes ~s p~rt of ~n ;;uto Sc~ling event using prebuilt ;;MIs. Use new versions of the ;;MIs to ~dd inst~nces. ~nd ph~se out ~ll inst~nces th~t use the previous ;;MI version with the con gured termin~tion policy during ~ deployment event.

 Correct ;;nswer: B
 B (100%)

 Question #87
 ;; comp~ny h~s ~n ~pplic~tion th~t runs on ;;m~zon  EC2 inst~nces. ;; solutions ~rchitect is designing VPC infr~structure in ~n ;;WS  Region where the ~pplic~tion needs to ~ccess ~n ;;m~zon ;;uror~  DB Cluster. The  EC2 inst~nces ~re ~ll ~ssoci~ted with the s~me security group. The  DB cluster is ~ssoci~ted with its own security group. The solutions ~rchitect needs to ~dd rules to the security groups to provide the ~pplic~tion with le~st privilege ~ccess to the  DB Cluster. Which combin~tion of steps will meet these requirements? (Choose two.)
  ;;. ;;dd ~n inbound rule to the  EC2 inst~nces' security group. Specify the  DB cluster's security group ~s the source over the def~ult ;;uror~ port.
  B. ;;dd ~n outbound rule to the  EC2 inst~nces' security group. Specify the  DB cluster's security group ~s the destin~tion over the def~ult ;;uror~ port.
  C. ;;dd ~n inbound rule to the  DB cluster's security group. Specify the  EC2 inst~nces' security group ~s the source over the def~ult ;;uror~ port.
  D. ;;dd ~n outbound rule to the  DB cluster's security group. Specify the  EC2 inst~nces' security group ~s the destin~tion over the def~ult ;;uror~ port.
  E. ;;dd ~n outbound rule to the  DB cluster's security group. Specify the  EC2 inst~nces' security group ~s the destin~tion over the ephemer~l ports.

 Correct ;;nswer: ;;B
 BC (73%)                                ;;C (27%)

 Question #88
 ;; comp~ny w~nts to ch~nge its intern~l cloud billing str~tegy for e~ch of its business units. Currently, the cloud govern~nce te~m sh~res reports for over~ll cloud spending with the he~d of e~ch business unit. The comp~ny uses ;;WS Org~niz~tions to m~n~ge the sep~r~te ;;WS ~ccounts for e~ch business unit. The existing t~gging st~nd~rd in Org~niz~tions includes the ~pplic~tion, environment, ~nd owner. The cloud govern~nce te~m w~nts ~ centr~lized solution so e~ch business unit receives monthly reports on its cloud spending. The solution should ~lso send noti c~tions for ~ny cloud spending th~t exceeds ~ set threshold. Which solution is the  MOST cost-effective w~y to meet these requirements?
  ;;. Con gure ;;WS  Budgets in e~ch ~ccount ~nd con gure budget ~lerts th~t ~re grouped by ~pplic~tion, environment, ~nd owner. ;;dd e~ch business unit to ~n ;;m~zon SNS topic for e~ch ~lert. Use Cost  Explorer in e~ch ~ccount to cre~te monthly reports for e~ch business unit.
  B. Con gure ;;WS  Budgets in the org~niz~tion's m~n~gement ~ccount ~nd con gure budget ~lerts th~t ~re grouped by ~pplic~tion, environment, ~nd owner. ;;dd e~ch business unit to ~n ;;m~zon SNS topic for e~ch ~lert. Use Cost  Explorer in the org~niz~tion's m~n~gement ~ccount to cre~te monthly reports for e~ch business unit.
  C. Con gure ;;WS  Budgets in e~ch ~ccount ~nd con gure budget ~lerts th~t ~re grouped by ~pplic~tion, environment, ~nd owner. ;;dd e~ch business unit to ~n ;;m~zon SNS topic for e~ch ~lert. Use the ;;WS  Billing ~nd Cost  M~n~gement d~shbo~rd in e~ch ~ccount to cre~te monthly reports for e~ch business unit.
  D.  En~ble ;;WS Cost ~nd Us~ge  Reports in the org~niz~tion's m~n~gement ~ccount ~nd con gure reports grouped by ~pplic~tion, environment. ~nd owner. Cre~te ~n ;;WS  L~mbd~ function th~t processes ;;WS Cost ~nd Us~ge  Reports, sends budget ~lerts, ~nd sends monthly reports to e~ch business unit's em~il list.

 Correct ;;nswer: B
 B (100%)

 Question #89
 ;; comp~ny is using ;;WS CloudForm~tion to deploy its infr~structure. The comp~ny is concerned th~t, if ~ production CloudForm~tion st~ck is deleted, import~nt d~t~ stored in ;;m~zon  RDS d~t~b~ses or ;;m~zon  EBS volumes might ~lso be deleted. How c~n the comp~ny prevent users from ~ccident~lly deleting d~t~ in this w~y?
  ;;.  Modify the CloudForm~tion templ~tes to ~dd ~  DeletionPolicy ~ttribute to  RDS ~nd  EBS resources.
  B. Con gure ~ st~ck policy th~t dis~llows the deletion of  RDS ~nd  EBS resources.
  C.  Modify  I;;M policies lo deny deleting  RDS ~nd  EBS resources th~t ~re t~gged with ~n "~ws:cloudform~tion:st~ck-n~me" t~g.
  D. Use ;;WS Con g rules to prevent deleting  RDS ~nd  EBS resources.

 Correct ;;nswer: ;;
 ;; (83%)                                  B (17%)

 Question #90
 ;; comp~ny h~s VPC  ow logs en~bled for  Its  N;;T g~tew~y. The comp~ny is seeing ;;ction = ;;CCEPT for inbound tr~ c th~t comes from public  IP ~ddress  198.51.100.2 destined for ~ priv~te ;;m~zon  EC2 inst~nce. ;; solutions ~rchitect must determine whether the tr~ c represents unsolicited inbound connections from the internet. The  rst two octets of the VPC CIDR block ~re 203.0. Which set of steps should the solutions ~rchitect t~ke to meet these requirements?
  ;;. Open the ;;WS CloudTr~il console. Select the log group th~t cont~ins the  N;;T g~tew~y's el~stic network interf~ce ~nd the priv~te inst~nce's el~stic network interl~ce.  Run ~ query to  lter with the destin~tion ~ddress set ~s "like 203.0" ~nd the source ~ddress set ~s "like 198.51.100.2".  Run the st~ts comm~nd to  lter the sum of bytes tr~nsferred by the source ~ddress ~nd the destin~tion ~ddress.
  B. Open the ;;m~zon CloudW~tch console. Select the log group th~t cont~ins the  N;;T g~tew~y's el~stic network interf~ce ~nd the priv~te inst~nce's el~stic network interf~ce.  Run ~ query to  lter with the destin~tion ~ddress set ~s "like 203.0" ~nd the source ~ddress set ~s "like 198.51.100.2".  Run the st~ts comm~nd to  lter the sum of bytes tr~nsferred by the source ~ddress ~nd the destin~tion ~ddress.
  C. Open the ;;WS CloudTr~il console. Select the log group th~t cont~ins the  N;;T g~tew~y's el~stic network interf~ce ~nd the priv~te inst~nce’s el~stic network interf~ce.  Run ~ query to  lter with the destin~tion ~ddress set ~s "like  198.51.100.2" ~nd the source ~ddress set ~s "like 203.0".  Run the st~ts comm~nd to  lter the sum of bytes tr~nsferred by the source ~ddress ~nd the destin~tion ~ddress.
  D. Open the ;;m~zon CloudW~tch console. Select the log group th~t cont~ins the  N;;T g~tew~y's el~stic network interf~ce ~nd the priv~te inst~nce's el~stic network interf~ce.  Run ~ query to  lter with the destin~tion ~ddress set ~s "like  198.51.100.2" ~nd the source ~ddress set ~s "like 203.0".  Run the st~ts comm~nd to  lter the sum of bytes tr~nsferred by the source ~ddress ~nd the destin~tion ~ddress.

 Correct ;;nswer: D
 B (65%)                                  D (35%)

 Question #91
 ;; comp~ny consists or two sep~r~te business units.  E~ch business unit h~s its own ;;WS ~ccount within ~ single org~niz~tion in ;;WS Org~niz~tions. The business units regul~rly sh~re sensitive documents with e~ch other. To f~cilit~te sh~ring, the comp~ny cre~ted ~n ;;m~zon S3 bucket in e~ch ~ccount ~nd con gured low-w~y replic~tion between the S3 buckets. The S3 buckets h~ve millions of objects. Recently, ~ security ~udit identi ed th~t neither S3 bucket h~s encryption ~t rest en~bled. Comp~ny policy requires th~t ~ll documents must be stored with encryption ~t rest. The comp~ny w~nts to implement server-side encryption with ;;m~zon S3 m~n~ged encryption keys (SSE-S3). Wh~t is the  MOST oper~tion~lly e cient solution th~t meets these requirements?
  ;;. Turn on SSE-S3 on both S3 buckets. Use S3  B~tch Oper~tions to copy ~nd encrypt the objects in the s~me loc~tion.
  B. Cre~te ~n ;;WS  Key  M~n~gement Service (;;WS  KMS) key in e~ch ~ccount. Turn on server-side encryption with ;;WS  KMS keys (SSE-KMS) on e~ch S3 bucket by using the corresponding  KMS key in th~t ;;WS ~ccount.  Encrypt the existing objects by using ~n S3 copy comm~nd in the ;;WS CLI.
  C. Turn on SSE-S3 on both S3 buckets.  Encrypt the existing objects by using ~n S3 copy comm~nd in the ;;WS CLI.
  D. Cre~te ~n ;;WS  Key  M~n~gement Service, (;;WS  KMS) key in e~ch ~ccount. Turn on server-side encryption with ;;WS  KMS keys (SSE-KMS) on e~ch S3 bucket by using the corresponding  KMS key in th~t ;;WS ~ccount. Use S3  B~tch Oper~tions to copy the objects into the s~me loc~tion.

 Correct ;;nswer: C
 ;; (88%)                                   10%

 Question #92
 ;; comp~ny is running ~n ~pplic~tion in the ;;WS Cloud. The ~pplic~tion collects ~nd stores ~ l~rge ~mount of unstructured d~t~ in ~n ;;m~zon S3 bucket. The S3 bucket cont~ins sever~l ter~bytes of d~t~ ~nd uses the S3 St~nd~rd stor~ge cl~ss. The d~t~ incre~ses in size by sever~l gig~bytes every d~y. The comp~ny needs to query ~nd ~n~lyze the d~t~. The comp~ny does not ~ccess d~t~ th~t is more th~n  1 ye~r old.  However, the comp~ny must ret~in ~ll the d~t~ inde nitely for compli~nce re~sons. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Use S3 Select to query the d~t~. Cre~te ~n S3  Lifecycle policy to tr~nsition d~t~ th~t is more th~n  1 ye~r old to S3 Gl~cier  Deep ;;rchive.
  B. Use ;;m~zon  Redshift Spectrum to query the d~t~. Cre~te ~n S3  Lifecycle policy to tr~nsition d~t~ th~t is more th~n  1 ye~r old  10 S3 Gl~cier Deep ;;rchive.
  C. Use ~n ;;WS Glue  D~t~ C~t~log ~nd ;;m~zon ;;then~ to query the d~t~. Cre~te ~n S3  Lifecycle policy to tr~nsition d~t~ th~t is more th~n  1 ye~r old to S3 Gl~cier  Deep ;;rchive.
  D. Use ;;m~zon  Redshift Spectrum to query the d~t~. Cre~te ~n S3  Lifecycle policy to tr~nsition d~t~ th~t is more th~n  1 ye~r old to S3 Intelligent-Tiering.

 Correct ;;nswer: ;;
 C (89%)                                   8%

 Question #93
 ;; video processing comp~ny w~nts to build ~ m~chine le~rning (ML) model by using 600 TB of compressed d~t~ th~t is stored ~s thous~nds of  les in the comp~ny's on-premises network ~tt~ched stor~ge system. The comp~ny does not h~ve the necess~ry compute resources on premises for  ML experiments ~nd w~nts to use ;;WS. The comp~ny needs to complete the d~t~ tr~nsfer to ;;WS within 3 weeks. The d~t~ tr~nsfer will be ~ one-time tr~nsfer. The d~t~ must be encrypted in tr~nsit. The me~sured uplo~d speed of the comp~ny's internet connection is  100  Mbps. ~nd multiple dep~rtments sh~re the connection. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Order sever~l ;;WS Snowb~ll  Edge Stor~ge Optimized devices by using the ;;WS  M~n~gement Console. Con gure the devices with ~ destin~tion S3 bucket. Copy the d~t~ to the devices. Ship the devices b~ck to ;;WS.
  B. Set up ~  10 Gbps ;;WS  Direct Connect connection between the comp~ny loc~tion ~nd the ne~rest ;;WS  Region. Tr~nsfer the d~t~ over ~ VPN connection into the  Region to store the d~t~ in ;;m~zon S3.
  C. Cre~te ~ VPN connection between the on-premises network ~tt~ched stor~ge ~nd the ne~rest ;;WS  Region. Tr~nsfer the d~t~ over the VPN connection.
  D.  Deploy ~n ;;WS Stor~ge G~tew~y  le g~tew~y on premises. Con gure the  le g~tew~y with ~ destin~tion S3 bucket. Copy the d~t~ to the  le g~tew~y.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #94
 ;; comp~ny h~s migr~ted  Its forms-processing ~pplic~tion to ;;WS. When users inter~ct with the ~pplic~tion, they uplo~d sc~nned forms ~s  les through ~ web ~pplic~tion. ;; d~t~b~se stores user met~d~t~ ~nd references to  les th~t ~re stored in ;;m~zon S3. The web ~pplic~tion runs on ;;m~zon  EC2 inst~nces ~nd ~n ;;m~zon  RDS for  PostgreSQL d~t~b~se. When forms ~re uplo~ded, the ~pplic~tion sends noti c~tions to ~ te~m through ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS). ;; te~m member then logs in ~nd processes e~ch form. The te~m member performs d~t~ v~lid~tion on the form ~nd extr~cts relev~nt d~t~ before entering the inform~tion into ~nother system th~t uses ~n ;;PI. ;; solutions ~rchitect needs to ~utom~te the m~nu~l processing of the forms. The solution must provide ~ccur~te form extr~ction. minimize time to m~rket, ~nd minimize tong-term oper~tion~l overhe~d. Which solution will meet these requirements?
  ;;.  Develop custom libr~ries to perform optic~l ch~r~cter recognition (OCR) on the forms.  Deploy the libr~ries to ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster ~s ~n ~pplic~tion tier. Use this tier to process the forms when forms ~re uplo~ded. Store the output in ;;m~zon S3.  P~rse this output by extr~cting the d~t~ into ~n ;;m~zon  Dyn~moDB t~ble. Submit the d~t~ to the t~rget system's ;;PL.  Host the new ~pplic~tion tier on  EC2 inst~nces.
  B.  Extend the system with ~n ~pplic~tion tier th~t uses ;;WS Step  Functions ~nd ;;WS  L~mbd~. Con gure this tier to use ~rti ci~l intelligence ~nd m~chine le~rning (;;I/ML) models th~t ~re tr~ined ~nd hosted on ~n  EC2 inst~nce to perform optic~l ch~r~cter recognition (OCR) on the forms when forms ~re uplo~ded. Store the output in ;;m~zon S3.  P~rse this output by extr~cting the d~t~ th~t is required within the ~pplic~tion tier. Submit the d~t~ to the t~rget system's ;;PI.
  C.  Host ~ new ~pplic~tion tier on  EC2 inst~nces. Use this tier to c~ll endpoints th~t host ~rti ci~l intelligence ~nd m~chine te~ming (;;I/ML) models th~t ~re tr~ined ~nd hosted in ;;m~zon S~geM~ker to perform optic~l ch~r~cter recognition (OCR) on the forms. Store the output in ;;m~zon  El~stiC~che.  P~rse this output by extr~cting the d~t~ th~t is required within the ~pplic~tion tier. Submit the d~t~ to the t~rget system's ;;PI.
  D.  Extend the system with ~n ~pplic~tion tier th~t uses ;;WS Step  Functions ~nd ;;WS  L~mbd~. Con gure this tier to use ;;m~zon Textr~ct ~nd ;;m~zon Comprehend to perform optic~l ch~r~cter recognition (OCR) on the forms when forms ~re uplo~ded. Store the output in ;;m~zon S3. P~rse this output by extr~cting the d~t~ th~t is required within the ~pplic~tion tier. Submit the d~t~ to the t~rget system's ;;PI.

 Correct ;;nswer: D
 D (100%)

 Question #95
 ;; comp~ny is ref~ctoring its on-premises order-processing pl~tform in the ;;WS Cloud. The pl~tform includes ~ web front end th~t is hosted on ~  eet of VMs,  R~bbitMQ to connect the front end to the b~ckend, ~nd ~  Kubernetes cluster to run ~ cont~inerized b~ckend system to process the orders. The comp~ny does not w~nt to m~ke ~ny m~jor ch~nges to the ~pplic~tion. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n ;;MI of the web server VM. Cre~te ~n ;;m~zon  EC2 ;;uto Sc~ling group th~t uses the ;;MI ~nd ~n ;;pplic~tion  Lo~d  B~l~ncer. Set up ;;m~zon  MQ to repl~ce the on-premises mess~ging queue. Con gure ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) to host the order- processing b~ckend.
  B. Cre~te ~ custom ;;WS  L~mbd~ runtime to mimic the web server environment. Cre~te ~n ;;m~zon ;;PI G~tew~y ;;PI to repl~ce the front-end web servers. Set up ;;m~zon  MQ to repl~ce the on-premises mess~ging queue. Con gure ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) to host the order-processing b~ckend.
  C. Cre~te ~n ;;MI of the web server VM. Cre~te ~n ;;m~zon  EC2 ;;uto Sc~ling group th~t uses the ;;MI ~nd ~n ;;pplic~tion  Lo~d  B~l~ncer. Set up ;;m~zon  MQ to repl~ce the on-premises mess~ging queue.  Inst~ll  Kubernetes on ~  eet of different  EC2 inst~nces to host the order- processing b~ckend.
  D. Cre~te ~n ;;MI of the web server VM. Cre~te ~n ;;m~zon  EC2 ;;uto Sc~ling group th~t uses the ;;MI ~nd ~n ;;pplic~tion  Lo~d  B~l~ncer. Set up ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue to repl~ce the on-premises mess~ging queue. Con gure ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) to host the order-processing b~ckend.

 Correct ;;nswer: ;;
 ;; (91%)                                   9%

 Question #96
 ;; solutions ~rchitect needs to implement ~ client-side encryption mech~nism for objects th~t will be stored in ~ new ;;m~zon S3 bucket. The solutions ~rchitect cre~ted ~ CMK th~t is stored in ;;WS  Key  M~n~gement Service (;;WS  KMS) for this purpose. The solutions ~rchitect cre~ted the following  I;;M policy ~nd ~tt~ched it to ~n  I;;M role: During tests, the solutions ~rchitect w~s ~ble to successfully get existing test objects in the S3 bucket.  However, ~ttempts to uplo~d ~ new object resulted in ~n error mess~ge. The error mess~ge st~ted th~t the ~ction w~s forbidden. Which ~ction must the solutions ~rchitect ~dd to the  I;;M policy to meet ~ll the requirements?
  ;;. kms:Gener~teD~t~Key
  B. kms:GetKeyPolicy
  C. kms:GetPublicKey
  D. kms:Sign

 Correct ;;nswer: ;;
 ;; (100%)

 Question #97
 ;; comp~ny h~s developed ~ web ~pplic~tion. The comp~ny is hosting the ~pplic~tion on ~ group of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion Lo~d  B~l~ncer. The comp~ny w~nts to improve the security posture of the ~pplic~tion ~nd pl~ns to use ;;WS W;;F web ;;CLs. The solution must not ~dversely ~ffect legitim~te tr~ c to the ~pplic~tion. How should ~ solutions ~rchitect con gure the web ;;CLs to meet these requirements?
  ;;. Set the ~ction of the web ;;CL rules to Count.  En~ble ;;WS W;;F logging. ;;n~lyze the requests for f~lse positives.  Modify the rules to ~void ~ny f~lse positive. Over time, ch~nge the ~ction of the web ;;CL rules from Count to  Block.
  B. Use only r~te-b~sed rules in the web ;;CLs, ~nd set the throttle limit ~s high ~s possible. Tempor~rily block ~ll requests th~t exceed the limit.  De ne nested rules to n~rrow the scope of the r~te tr~cking.
  C. Set the ~ction of the web ;;CL rules to  Block. Use only ;;WS m~n~ged rule groups in the web ;;CLs.  Ev~lu~te the rule groups by using ;;m~zon CloudW~tch metrics with ;;WS W;;F s~mpled requests or ;;WS W;;F logs.
  D. Use only custom rule groups in the web ;;CLs, ~nd set the ~ction to ;;llow.  En~ble ;;WS W;;F logging. ;;n~lyze the requests for f~lse positives.  Modify the rules to ~void ~ny f~lse positive. Over time, ch~nge the ~ction of the web ;;CL rules from ;;llow to  Block.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #98
 ;; comp~ny h~s ~n org~niz~tion th~t h~s m~ny ;;WS ~ccounts in ;;WS Org~niz~tions. ;; solutions ~rchitect must improve how the comp~ny m~n~ges common security group rules for the ;;WS ~ccounts in the org~niz~tion. The comp~ny h~s ~ common set of  IP CIDR r~nges in ~n ~llow list in e~ch ;;WS ~ccount to ~llow ~ccess to ~nd from the comp~ny’s on-premises network.  Developers within e~ch ~ccount ~re responsible for ~dding new  IP CIDR r~nges to their security groups. The security te~m h~s its own ;;WS ~ccount. Currently, the security te~m noti es the owners of the other ;;WS ~ccounts when ch~nges ~re m~de to the ~llow list. The solutions ~rchitect must design ~ solution th~t distributes the common set of CIDR r~nges ~cross ~ll ~ccounts. Which solution meets these requirements with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;. Set up ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic in the security te~m's ;;WS ~ccount.  Deploy ~n ;;WS  L~mbd~ function in e~ch ;;WS ~ccount. Con gure the  L~mbd~ function to run every time ~n SNS topic receives ~ mess~ge. Con gure the  L~mbd~ function to t~ke ~n  IP ~ddress ~s input ~nd ~dd it to ~ list of security groups in the ~ccount.  Instruct the security te~m to distribute ch~nges by publishing mess~ges to its SNS topic.
  B. Cre~te new customer-m~n~ged pre x lists in e~ch ;;WS ~ccount within the org~niz~tion.  Popul~te the pre x lists in e~ch ~ccount with ~ll intern~l CIDR r~nges.  Notify the owner of e~ch ;;WS ~ccount to ~llow the new customer-m~n~ged pre x list  IDs in their ~ccounts in their security groups.  Instruct the security te~m to sh~re upd~tes with e~ch ;;WS ~ccount owner.
  C. Cre~te ~ new customer-m~n~ged pre x list in the security te~m’s ;;WS ~ccount.  Popul~te the customer-m~n~ged pre x list with ~ll intern~l CIDR r~nges. Sh~re the customer-m~n~ged pre x list with the org~niz~tion by using ;;WS  Resource ;;ccess  M~n~ger.  Notify the owner of e~ch ;;WS ~ccount to ~llow the new customer-m~n~ged pre x list  ID in their security groups.
  D. Cre~te ~n  I;;M role in e~ch ~ccount in the org~niz~tion. Gr~nt permissions to upd~te security groups.  Deploy ~n ;;WS  L~mbd~ function in the security te~m’s ;;WS ~ccount. Con gure the  L~mbd~ function to t~ke ~ list of intern~l  IP ~ddresses ~s input, ~ssume ~ role in e~ch org~niz~tion ~ccount, ~nd ~dd the list of  IP ~ddresses to the security groups in e~ch ~ccount.

 Correct ;;nswer: C
 C (88%)                                   13%

 Question #99
 ;; comp~ny h~s introduced ~ new policy th~t ~llows employees to work remotely from their homes if they connect by using ~ VPN. The comp~ny is hosting intern~l ~pplic~tions with VPCs in multiple ;;WS ~ccounts. Currently, the ~pplic~tions ~re ~ccessible from the comp~ny's on-premises o ce network through ~n ;;WS Site-to-Site VPN connection. The VPC in the comp~ny's m~in ;;WS ~ccount h~s peering connections est~blished with VPCs in other ;;WS ~ccounts. ;; solutions ~rchitect must design ~ sc~l~ble ;;WS Client VPN solution for employees to use while they work from home. Wh~t is the  MOST cost-effective solution th~t meets these requirements?
  ;;. Cre~te ~ Client VPN endpoint in e~ch ;;WS ~ccount. Con gure required routing th~t ~llows ~ccess to intern~l ~pplic~tions.
  B. Cre~te ~ Client VPN endpoint in the m~in ;;WS ~ccount. Con gure required routing th~t ~llows ~ccess to intern~l ~pplic~tions.
  C. Cre~te ~ Client VPN endpoint in the m~in ;;WS ~ccount.  Provision ~ tr~nsit g~tew~y th~t is connected to e~ch ;;WS ~ccount. Con gure required routing th~t ~llows ~ccess to intern~l ~pplic~tions.
  D. Cre~te ~ Client VPN endpoint in the m~in ;;WS ~ccount.  Est~blish connectivity between the Client VPN endpoint ~nd the ;;WS Site-to-Site VPN.

 Correct ;;nswer: B
 C (53%)                                 B (47%)

 Question #100
 ;; comp~ny is running ~n ~pplic~tion in the ;;WS Cloud.  Recent ~pplic~tion metrics show inconsistent response times ~nd ~ signi c~nt incre~se in error r~tes. C~lls to third-p~rty services ~re c~using the del~ys. Currently, the ~pplic~tion c~lls third-p~rty services synchronously by directly invoking ~n ;;WS  L~mbd~ function. ;; solutions ~rchitect needs to decouple the third-p~rty service c~lls ~nd ensure th~t ~ll the c~lls ~re eventu~lly completed. Which solution will meet these requirements?
  ;;. Use ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue to store events ~nd invoke the  L~mbd~ function.
  B. Use ~n ;;WS Step  Functions st~te m~chine to p~ss events to the  L~mbd~ function.
  C. Use ~n ;;m~zon  EventBridge rule to p~ss events to the  L~mbd~ function.
  D. Use ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic to store events ~nd  Invoke the  L~mbd~ function.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #101
 ;; comp~ny is running ~pplic~tions on ;;WS in ~ multi-~ccount environment. The comp~ny's s~les te~m ~nd m~rketing te~m use sep~r~te ;;WS ~ccounts in ;;WS Org~niz~tions. The s~les te~m stores pet~bytes of d~t~ in ~n ;;m~zon S3 bucket. The m~rketing te~m uses ;;m~zon QuickSight for d~t~ visu~liz~tions. The m~rketing te~m needs ~ccess to d~t~ th~t the s~tes te~m stores in the S3 bucket. The comp~ny h~s encrypted the S3 bucket with ~n ;;WS  Key M~n~gement Service (;;WS  KMS) key. The m~rketing te~m h~s ~lre~dy cre~ted the  I;;M service role for QuickSight to provide QuickSight ~ccess in the m~rketing ;;WS ~ccount. The comp~ny needs ~ solution th~t will provide secure ~ccess to the d~t~ in the S3 bucket ~cross ;;WS ~ccounts. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ new S3 bucket in the m~rketing ~ccount. Cre~te ~n S3 replic~tion rule in the s~les ~ccount to copy the objects to the new S3 bucket in the m~rketing ~ccount. Upd~te the QuickSight permissions in the m~rketing ~ccount to gr~nt ~ccess to the new S3 bucket.
  B. Cre~te ~n SCP to gr~nt ~ccess to the S3 bucket to the m~rketing ~ccount. Use ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M) to sh~re the KMS key from the s~tes ~ccount with the m~rketing ~ccount. Upd~te the QuickSight permissions in the m~rketing ~ccount to gr~nt ~ccess to the S3 bucket.
  C. Upd~te the S3 bucket policy in the m~rketing ~ccount to gr~nt ~ccess to the QuickSight role. Cre~te ~  KMS gr~nt for the encryption key th~t is used in the S3 bucket. Gr~nt decrypt ~ccess to the QuickSight role. Upd~te the QuickSight permissions in the m~rketing ~ccount to gr~nt ~ccess to the S3 bucket.
  D. Cre~te ~n  I;;M role in the s~les ~ccount ~nd gr~nt ~ccess to the S3 bucket.  From the m~rketing ~ccount, ~ssume the  I;;M role in the s~les ~ccount to ~ccess the S3 bucket. Upd~te the QuickSight rote, to cre~te ~ trust rel~tionship with the new  I;;M role in the s~les ~ccount.

 Correct ;;nswer: D
 D (73%)                            13%        12%

 Question #102
 ;; comp~ny is pl~nning to migr~te its business-critic~l ~pplic~tions from ~n on-premises d~t~ center to ;;WS. The comp~ny h~s ~n on-premises inst~ll~tion of ~  Microsoft SQL Server ;;lw~ys On cluster. The comp~ny w~nts to migr~te to ~n ;;WS m~n~ged d~t~b~se service. ;; solutions ~rchitect must design ~ heterogeneous d~t~b~se migr~tion on ;;WS. Which solution will meet these requirements?
  ;;.  Migr~te the SQL Server d~t~b~ses to ;;m~zon  RDS for  MySQL by using b~ckup ~nd restore utilities.
  B. Use ~n ;;WS Snowb~ll  Edge Stor~ge Optimized device to tr~nsfer d~t~ to ;;m~zon S3. Set up ;;m~zon  RDS for  MySQL. Use S3 integr~tion with SQL Server fe~tures, such ~s  BULK  INSERT.
  C. Use the ;;WS Schem~ Conversion Tool to tr~nsl~te the d~t~b~se schem~ to ;;m~zon  RDS for  MySQL. Then use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to migr~te the d~t~ from on-premises d~t~b~ses to ;;m~zon  RDS.
  D. Use ;;WS  D~t~Sync to migr~te d~t~ over the network between on-premises stor~ge ~nd ;;m~zon S3. Set up ;;m~zon  RDS for  MySQL. Use S3 integr~tion with SQL Server fe~tures, such ~s  BULK  INSERT.

 Correct ;;nswer: C
 C (100%)

 Question #103
 ;; publishing comp~ny's design te~m upd~tes the icons ~nd other st~tic ~ssets th~t ~n ecommerce web ~pplic~tion uses. The comp~ny serves the icons ~nd ~ssets from ~n ;;m~zon S3 bucket th~t is hosted in the comp~ny's production ~ccount. The comp~ny ~lso uses ~ development ~ccount th~t members of the design te~m c~n ~ccess. ;;fter the design te~m tests the st~tic ~ssets in the development ~ccount, the design te~m needs to lo~d the ~ssets into the S3 bucket in the production ~ccount. ;; solutions ~rchitect must provide the design te~m with ~ccess to the production ~ccount without exposing other p~rts of the web ~pplic~tion to the risk of unw~nted ch~nges. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;.  In the production ~ccount, cre~te ~ new  I;;M policy th~t ~llows re~d ~nd write ~ccess to the S3 bucket.
  B.  In the development ~ccount, cre~te ~ new  I;;M policy th~t ~llows re~d ~nd write ~ccess to the S3 bucket.
  C.  In the production ~ccount, cre~te ~ role ;;tt~ch the new policy to the role.  De ne the development ~ccount ~s ~ trusted entity.
  D.  In the development ~ccount, cre~te ~ role. ;;tt~ch the new policy to the role  De ne the production ~ccount ~s ~ trusted entity.
  E.  In the development ~ccount, cre~te ~ group th~t cont~ins ~ll the  I;;M users of the design te~m ;;tt~ch ~ different  I;;M policy to the group to ~llow the sts:;;ssumeRole ~ction on the role  In the production ~ccount.
  F.  In the development ~ccount, cre~te ~ group th~t cont~ins ~ll the  I;;M users of the design te~m ;;tt~ch ~ different  I;;M policy to the group to ~llow the sts:;;ssumeRole ~ction on the role in the development ~ccount.

 Correct ;;nswer: ;;DE
 ;;CE (94%)                                  6%

 Question #104
 ;; comp~ny developed ~ pilot ~pplic~tion by using ;;WS  El~stic  Be~nst~lk ~nd J~v~. To s~ve costs during development, the comp~ny's development te~m deployed the ~pplic~tion into ~ single-inst~nce environment.  Recent tests indic~te th~t the ~pplic~tion consumes more CPU th~n expected. CPU utiliz~tion is regul~rly gre~ter th~n 85%, which c~uses some perform~nce bottlenecks. ;; solutions ~rchitect must mitig~te the perform~nce issues before the comp~ny l~unches the ~pplic~tion to production. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ new  El~stic  Be~nst~lk ~pplic~tion. Select ~ lo~d-b~l~nced environment type. Select ~ll ;;v~il~bility Zones. ;;dd ~ sc~le-out rule th~t will run if the m~ximum CPU utiliz~tion is over 85% for 5 minutes.
  B. Cre~te ~ second  El~stic  Be~nst~lk environment. ;;pply the tr~ c-splitting deployment policy. Specify ~ percent~ge of incoming tr~ c to direct to the new environment in the ~ver~ge CPU utiliz~tion is over 85% for 5 minutes.
  C.  Modify the existing environment’s c~p~city con gur~tion to use ~ lo~d-b~l~nced environment type. Select ~ll ;;v~il~bility Zones. ;;dd ~ sc~le-out rule th~t will run if the ~ver~ge CPU utiliz~tion is over 85% for 5 minutes.
  D. Select the  Rebuild environment ~ction with the lo~d b~l~ncing option. Select ~n ;;v~il~bility Zones. ;;dd ~ sc~le-out rule th~t will run if the sum CPU utiliz~tion is over 85% for 5 minutes.

 Correct ;;nswer: ;;
 C (95%)                                     5%

 Question #105
 ;;  n~nce comp~ny is running its business-critic~l ~pplic~tion on current-gener~tion  Linux  EC2 inst~nces. The ~pplic~tion includes ~ self-m~n~ged MySQL d~t~b~se performing he~vy  I/O oper~tions. The ~pplic~tion is working  ne to h~ndle ~ moder~te ~mount of tr~ c during the month. However, it slows down during the  n~l three d~ys of e~ch month due to month-end reporting, even though the comp~ny is using  El~stic  Lo~d B~l~ncers ~nd ;;uto Sc~ling within its infr~structure to meet the incre~sed dem~nd. Which of the following ~ctions would ~llow the d~t~b~se to h~ndle the month-end lo~d with the  LE;;ST imp~ct on perform~nce?
  ;;.  Pre-w~rming  El~stic  Lo~d  B~l~ncers, using ~ bigger inst~nce type, ch~nging ~ll ;;m~zon  EBS volumes to GP2 volumes.
  B.  Performing ~ one-time migr~tion of the d~t~b~se cluster to ;;m~zon  RDS, ~nd cre~ting sever~l ~ddition~l re~d replic~s to h~ndle the lo~d during end of month.
  C. Using ;;m~zon CloudW~tch with ;;WS  L~mbd~ to ch~nge the type, size, or  IOPS of ;;m~zon  EBS volumes in the cluster b~sed on ~ speci c CloudW~tch metric.
  D.  Repl~cing ~ll existing ;;m~zon  EBS volumes with new  PIOPS volumes th~t h~ve the m~ximum ~v~il~ble stor~ge size ~nd  I/O per second by t~king sn~pshots before the end of the month ~nd reverting b~ck ~fterw~rds.

 Correct ;;nswer: B
 B (92%)                                     8%

 Question #106
 ;; comp~ny runs ~ J~v~ ~pplic~tion th~t h~s complex dependencies on VMs th~t ~re in the comp~ny's d~t~ center. The ~pplic~tion is st~ble. but the comp~ny w~nts to modernize the technology st~ck. The comp~ny w~nts to migr~te the ~pplic~tion to ;;WS ~nd minimize the ~dministr~tive overhe~d to m~int~in the servers. Which solution will meet these requirements with the  LE;;ST code ch~nges?
  ;;.  Migr~te the ~pplic~tion to ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ;;WS  F~rg~te by using ;;WS ;;pp2Cont~iner. Store cont~iner im~ges in ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). Gr~nt the  ECS t~sk execution role permission  10 ~ccess the  ECR im~ge repository. Con gure ;;m~zon  ECS to use ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Use the ;;LB to inter~ct with the ~pplic~tion.
  B.  Migr~te the ~pplic~tion code to ~ cont~iner th~t runs in ;;WS  L~mbd~.  Build ~n ;;m~zon ;;PI G~tew~y  REST ;;PI with  L~mbd~ integr~tion. Use ;;PI G~tew~y to inter~ct with the ~pplic~tion.
  C.  Migr~te the ~pplic~tion to ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) on  EKS m~n~ged node groups by using ;;WS ;;pp2Cont~iner. Store cont~iner im~ges in ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). Give the  EKS nodes permission to ~ccess the  ECR im~ge repository. Use ;;m~zon ;;PI G~tew~y to inter~ct with the ~pplic~tion.
  D.  Migr~te the ~pplic~tion code to ~ cont~iner th~t runs in ;;WS  L~mbd~. Con gure  L~mbd~ to use ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Use the ;;LB to inter~ct with the ~pplic~tion.

 Correct ;;nswer: B
 ;; (91%)                                   9%

 Question #107
 ;; comp~ny h~s ~n ~synchronous  HTTP ~pplic~tion th~t is hosted ~s ~n ;;WS  L~mbd~ function. ;; public ;;m~zon ;;PI G~tew~y endpoint invokes the  L~mbd~ function. The  L~mbd~ function ~nd the ;;PI G~tew~y endpoint reside in the us-e~st-1  Region. ;; solutions ~rchitect needs to redesign the ~pplic~tion to support f~ilover to ~nother ;;WS  Region. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;PI G~tew~y endpoint in the us-west-2  Region to direct tr~ c to the  L~mbd~ function in us-e~st-1. Con gure ;;m~zon  Route 53 to use ~ f~ilover routing policy to route tr~ c for the two ;;PI G~tew~y endpoints.
  B. Cre~te ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Con gure ;;PI G~tew~y to direct tr~ c to the SQS queue inste~d of to the L~mbd~ function. Con gure the  L~mbd~ function to pull mess~ges from the queue for processing.
  C.  Deploy the  L~mbd~ function to the us-west-2  Region. Cre~te ~n ;;PI G~tew~y endpoint in us-west-2  10 direct tr~ c to the  L~mbd~ function in us-west-2. Con gure ;;WS Glob~l ;;cceler~tor ~nd ~n ;;pplic~tion  Lo~d  B~l~ncer to m~n~ge tr~ c ~cross the two ;;PI G~tew~y endpoints.
  D.  Deploy the  L~mbd~ function ~nd ~n ;;PI G~tew~y endpoint to the us-west-2  Region. Con gure ;;m~zon  Route 53 to use ~ f~ilover routing policy to route tr~ c for the two ;;PI G~tew~y endpoints.

 Correct ;;nswer: B
 D (93%)                                    7%

 Question #108
 ;; ret~il comp~ny h~s structured its ;;WS ~ccounts to be p~rt of ~n org~niz~tion in ;;WS Org~niz~tions. The comp~ny h~s set up consolid~ted billing ~nd h~s m~pped its dep~rtments to the following OUs:  Fin~nce, S~les,  Hum~n  Resources (HR),  M~rketing, ~nd Oper~tions.  E~ch OU h~s multiple ;;WS ~ccounts, one for e~ch environment within ~ dep~rtment. These environments ~re development, test, pre-production, ~nd production. The  HR dep~rtment is rele~sing ~ new system th~t will l~unch in 3 months.  In prep~r~tion, the  HR dep~rtment h~s purch~sed sever~l  Reserved Inst~nces (RIs) in its production ;;WS ~ccount. The  HR dep~rtment will inst~ll the new ~pplic~tion on this ~ccount. The  HR dep~rtment w~nts to m~ke sure th~t other dep~rtments c~nnot sh~re the  RI discounts. Which solution will meet these requirements?
  ;;.  In the ;;WS  Billing ~nd Cost  M~n~gement console for the  HR dep~rtment's production ~ccount turn off  RI sh~ring.
  B.  Remove the  HR dep~rtment's production ;;WS ~ccount from the org~niz~tion. ;;dd the ~ccount  10 the consolid~ting billing con gur~tion only.
  C.  In the ;;WS  Billing ~nd Cost  M~n~gement console. use the org~niz~tion’s m~n~gement ~ccount  10 turn off  RI Sh~ring for the  HR dep~rtments production ;;WS ~ccount.
  D. Cre~te ~n SCP in the org~niz~tion to restrict ~ccess to the  RIs. ;;pply the SCP to the OUs of the other dep~rtments.

 Correct ;;nswer: C
 C (87%)                                    13%

 Question #109
 ;; l~rge comp~ny is running ~ popul~r web ~pplic~tion. The ~pplic~tion runs on sever~l ;;m~zon  EC2  Linux inst~nces in ~n ;;uto Sc~ling group in ~ priv~te subnet. ;;n ;;pplic~tion  Lo~d  B~l~ncer is t~rgeting the inst~nces in the ;;uto Sc~ling group in the priv~te subnet. ;;WS Systems  M~n~ger Session  M~n~ger is con gured, ~nd ;;WS Systems  M~n~ger ;;gent is running on ~ll the  EC2 inst~nces. The comp~ny recently rele~sed ~ new version of the ~pplic~tion. Some  EC2 inst~nces ~re now being m~rked ~s unhe~lthy ~nd ~re being termin~ted. ;;s ~ result, the ~pplic~tion is running ~t reduced c~p~city. ;; solutions ~rchitect tries to determine the root c~use by ~n~lyzing ;;m~zon CloudW~tch logs th~t ~re collected from the ~pplic~tion, but the logs ~re inconclusive. How should the solutions ~rchitect g~in ~ccess to ~n  EC2 inst~nce to troubleshoot the issue?
  ;;. Suspend the ;;uto Sc~ling group’s  He~lthCheck sc~ling process. Use Session  M~n~ger to log in to ~n inst~nce th~t is m~rked ~s unhe~lthy.
  B.  En~ble  EC2 inst~nce termin~tion protection. Use Session  M~n~ger to log in to ~n inst~nce th~t is m~rked ~s unhe~lthy.
  C. Set the termin~tion policy to OldestInst~nce on the ;;uto Sc~ling group. Use Session  M~n~ger to log in to ~n inst~nce th~t is m~rked ~n unhe~lthy.
  D. Suspend the ;;uto Sc~ling group’s Termin~te process. Use Session  M~n~ger to log in to ~n inst~nce th~t is m~rked ~s unhe~lthy.

 Correct ;;nswer: D
 D (92%)                                     8%

 Question #110
 ;; comp~ny w~nts to deploy ~n ;;WS W;;F solution to m~n~ge ;;WS W;;F rules ~cross multiple ;;WS ~ccounts. The ~ccounts ~re m~n~ged under different OUs in ;;WS Org~niz~tions. ;;dministr~tors must be ~ble to ~dd or remove ~ccounts or OUs from m~n~ged ;;WS W;;F rule sets ~s needed. ;;dministr~tors ~lso must h~ve the ~bility to ~utom~tic~lly upd~te ~nd remedi~te noncompli~nt ;;WS W;;F rules in ~ll ~ccounts. Which solution meets these requirements with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;. Use ;;WS  Firew~ll  M~n~ger to m~n~ge ;;WS W;;F rules ~cross ~ccounts in the org~niz~tion. Use ~n ;;WS Systems  M~n~ger  P~r~meter Store p~r~meter to store ~ccount numbers ~nd OUs to m~n~ge. Upd~te the p~r~meter ~s needed to ~dd or remove ~ccounts or OUs. Use ~n ;;m~zon EventBridge rule to identify ~ny ch~nges to the p~r~meter ~nd to invoke ~n ;;WS  L~mbd~ function to upd~te the security policy in the  Firew~ll M~n~ger ~dministr~tive ~ccount.
  B.  Deploy ~n org~niz~tion-wide ;;WS Con g rule th~t requires ~ll resources in the selected OUs to ~ssoci~te the ;;WS W;;F rules.  Deploy ~utom~ted remedi~tion ~ctions by using ;;WS  L~mbd~ to  x noncompli~nt resources.  Deploy ;;WS W;;F rules by using ~n ;;WS CloudForm~tion st~ck set to t~rget the s~me OUs where the ;;WS Con g rule is ~pplied.
  C. Cre~te ;;WS W;;F rules in the m~n~gement ~ccount of the org~niz~tion. Use ;;WS  L~mbd~ environment v~ri~bles to store ~ccount numbers ~nd OUs to m~n~ge. Upd~te environment v~ri~bles ~s needed to ~dd or remove ~ccounts or OUs. Cre~te cross-~ccount  I;;M roles in member ~ccounts. ;;ssume the roles by using ;;WS Security Token Service (;;WS STS) in the  L~mbd~ function to cre~te ~nd upd~te ;;WS W;;F rules in the member ~ccounts.
  D. Use ;;WS Control Tower to m~n~ge ;;WS W;;F rules ~cross ~ccounts in the org~niz~tion. Use ;;WS  Key  M~n~gement Service (;;WS  KMS) to store ~ccount numbers ~nd OUs to m~n~ge. Upd~te ;;WS  KMS ~s needed to ~dd or remove ~ccounts or OUs. Cre~te  I;;M users in member ~ccounts. ;;llow ;;WS Control Tower in the m~n~gement ~ccount to use the ~ccess key ~nd secret ~ccess key to cre~te ~nd upd~te ;;WS W;;F rules in the member ~ccounts.

 Correct ;;nswer: D
 ;; (100%)

 Question #111
 ;; solutions ~rchitect is ~uditing the security setup or ~n ;;WS  L~mbd~ function for ~ comp~ny. The  L~mbd~ function retrieves, the l~test ch~nges from ~n ;;m~zon ;;uror~ d~t~b~se. The  L~mbd~ function ~nd the d~t~b~se run in the s~me VPC.  L~mbd~ environment v~ri~bles ~re providing the d~t~b~se credenti~ls to the  L~mbd~ function. The  L~mbd~ function ~ggreg~tes d~t~ ~nd m~kes the d~t~ ~v~il~ble in ~n ;;m~zon S3 bucket th~t is con gured for server-side encryption with ;;WS  KMS m~n~ged encryption keys (SSE-KMS). The d~t~ must not tr~vel ~cross the  Internet.  If ~ny d~t~b~se credenti~ls become compromised, the comp~ny needs ~ solution th~t minimizes the imp~ct of the compromise. Wh~t should the solutions ~rchitect recommend to meet these requirements?
  ;;.  En~ble  I;;M d~t~b~se ~uthentic~tion on the ;;uror~  DB cluster. Ch~nge the  I;;M role for the  L~mbd~ function to ~llow the function to ~ccess the d~t~b~se by using  I;;M d~t~b~se ~uthentic~tion.  Deploy ~ g~tew~y VPC endpoint for ;;m~zon S3 in the VPC.
  B.  En~ble  I;;M d~t~b~se ~uthentic~tion on the ;;uror~  DB cluster. Ch~nge the  I;;M role for the  L~mbd~ function to ~llow the function to ~ccess the d~t~b~se by using  I;;M d~t~b~se ~uthentic~tion.  Enforce  HTTPS on the connection to ;;m~zon S3 during d~t~ tr~nsfers.
  C. S~ve the d~t~b~se credenti~ls in ;;WS Systems  M~n~ger  P~r~meter Store. Set up p~ssword rot~tion on the credenti~ls in  P~r~meter Store. Ch~nge the  I;;M role for the  L~mbd~ function to ~llow the function to ~ccess  P~r~meter Store.  Modify the  L~mbd~ function to retrieve the credenti~ls from  P~r~meter Store.  Deploy ~ g~tew~y VPC endpoint for ;;m~zon S3 in the VPC.
  D. S~ve the d~t~b~se credenti~ls in ;;WS Secrets  M~n~ger. Set up p~ssword rot~tion on the credenti~ls in Secrets  M~n~ger. Ch~nge the  I;;M role for the  L~mbd~ function to ~llow the function to ~ccess Secrets  M~n~ger.  Modify the  L~mbd~ function to retrieve the credenti~ls from Secrets  M~n~ger.  Enforce  HTTPS on the connection to ;;m~zon S3 during d~t~ tr~nsfers.

 Correct ;;nswer: D
 ;; (85%)                                  D (15%)

 Question #112
 ;; l~rge mobile g~ming comp~ny h~s successfully migr~ted ~ll of its on-premises infr~structure to the ;;WS Cloud. ;; solutions ~rchitect is reviewing the environment to ensure th~t it w~s built ~ccording to the design ~nd th~t it is running in ~lignment with the Well-;;rchitected Fr~mework. While reviewing previous monthly costs in Cost  Explorer, the solutions ~rchitect notices th~t the cre~tion ~nd subsequent termin~tion of sever~l l~rge inst~nce types ~ccount for ~ high proportion of the costs. The solutions ~rchitect  nds out th~t the comp~ny’s developers ~re l~unching new ;;m~zon  EC2 inst~nces ~s p~rt of their testing ~nd th~t the developers ~re not using the ~ppropri~te inst~nce types. The solutions ~rchitect must implement ~ control mech~nism to limit the inst~nce types th~t only the developers c~n l~unch. Which solution will meet these requirements?
  ;;. Cre~te ~ desired-inst~nce-type m~n~ged rule in ;;WS Con g. Con gure the rule with the inst~nce types th~t ~re ~llowed. ;;tt~ch the rule to ~n event to run e~ch time ~ new  EC2 inst~nce is l~unched.
  B.  In the  EC2 console, cre~te ~ l~unch templ~te th~t speci es the inst~nce types th~t ~re ~llowed. ;;ssign the l~unch templ~te to the developers’  I;;M ~ccounts.
  C. Cre~te ~ new  I;;M policy. Specify the inst~nce types th~t ~re ~llowed. ;;tt~ch the policy to ~n  I;;M group th~t cont~ins the  I;;M ~ccounts for the developers
  D. Use  EC2  Im~ge  Builder to cre~te ~n im~ge pipeline for the developers ~nd ~ssist them in the cre~tion of ~ golden im~ge.

 Correct ;;nswer: C
 C (100%)

 Question #113
 ;; comp~ny is developing ~nd hosting sever~l projects in the ;;WS Cloud. The projects ~re developed ~cross multiple ;;WS ~ccounts under the s~me org~niz~tion in ;;WS Org~niz~tions. The comp~ny requires the cost for cloud infr~structure to be ~lloc~ted to the owning project. The te~m responsible for ~ll of the ;;WS ~ccounts h~s discovered th~t sever~l ;;m~zon  EC2 inst~nces ~re l~cking the  Project t~g used for cost ~lloc~tion. Which ~ctions should ~ solutions ~rchitect l~ke to resolve the problem ~nd prevent it from h~ppening in the future? (Choose three.)
  ;;. Cre~te ~n ;;WS Con g rule in e~ch ~ccount to  nd resources with missing t~gs.
  B. Cre~te ~n SCP in the org~niz~tion with ~ deny ~ction for ec2:RunInst~nces if the  Project t~g is missing.
  C. Use ;;m~zon  Inspector in the org~niz~tion to  nd resources with missing t~gs.
  D. Cre~te ~n  I;;M policy in e~ch ~ccount with ~ deny ~ction for ec2:RunInst~nces if the  Project t~g is missing.
  E. Cre~te ~n ;;WS Con g ~ggreg~tor for the org~niz~tion to collect ~ list of  EC2 inst~nces with the missing  Project t~g.
  F. Use ;;WS Security  Hub to ~ggreg~te ~ list of  EC2 inst~nces with the missing  Project t~g.

 Correct ;;nswer: CDE
 ;;BE (88%)                                  8%

 Question #114
 ;; comp~ny h~s ~n on-premises monitoring solution using ~  PostgreSQL d~t~b~se for persistence of events. The d~t~b~se is un~ble to sc~le due to he~vy ingestion ~nd it frequently runs out of stor~ge. The comp~ny w~nts to cre~te ~ hybrid solution ~nd h~s ~lre~dy set up ~ VPN connection between its network ~nd ;;WS. The solution should include the following ~ttributes: •  M~n~ged ;;WS services to minimize oper~tion~l complexity. • ;; buffer th~t ~utom~tic~lly sc~les to m~tch the throughput of d~t~ ~nd requires no ongoing ~dministr~tion. • ;; visu~liz~tion tool to cre~te d~shbo~rds to observe events in ne~r-re~l time. • Support for semi-structured JSON d~t~ ~nd dyn~mic schem~s. Which combin~tion of components will en~ble the comp~ny to cre~te ~ monitoring solution th~t will s~tisfy these requirements? (Choose two.)
  ;;. Use ;;m~zon  Kinesis  D~t~  Firehose to buffer events. Cre~te ~n ;;WS  L~mbd~ function to process ~nd tr~nsform events.
  B. Cre~te ~n ;;m~zon  Kinesis d~t~ stre~m to buffer events. Cre~te ~n ;;WS  L~mbd~ function to process ~nd tr~nsform events.
  C. Con gure ~n ;;m~zon ;;uror~  PostgreSQL  DB cluster to receive events. Use ;;m~zon QuickSight to re~d from the d~t~b~se ~nd cre~te ne~r- re~l-time visu~liz~tions ~nd d~shbo~rds.
  D. Con gure ;;m~zon  El~sticse~rch Service (;;m~zon  ES) to receive events. Use the  Kib~n~ endpoint deployed with ;;m~zon  ES to cre~te ne~r- re~l-time visu~liz~tions ~nd d~shbo~rds.
  E. Con gure ~n ;;m~zon  Neptune  DB inst~nce to receive events. Use ;;m~zon QuickSight to re~d from the d~t~b~se ~nd cre~te ne~r-re~l-time visu~liz~tions ~nd d~shbo~rds.

 Correct ;;nswer: ;;D
 ;;D (100%)

 Question #115
 ;; te~m collects ~nd routes beh~vior~l d~t~ for ~n entire comp~ny. The comp~ny runs ~  Multi-;;Z VPC environment with public subnets, priv~te subnets, ~nd in internet g~tew~y.  E~ch public subnet ~lso cont~ins ~  N;;T g~tew~y.  Most of the comp~ny’s ~pplic~tions re~d from ~nd write to ;;m~zon  Kinesis  D~t~ Stre~ms.  Most of the worklo~ds run in priv~te subnets. ;; solutions ~rchitect must review the infr~structure. The solution ~rchitect needs to reduce costs ~nd m~int~in the function of the ~pplic~tions. The solutions ~rchitect uses Cost  Explorer ~nd notices th~t the cost in the  EC2-Other c~tegory is consistently high. ;; further review shows th~t N~tG~tew~y-Bytes ch~rges ~re incre~sing the cost in the  EC2-Other c~tegory. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;.  En~ble VPC  Flow  Logs. Use ;;m~zon ;;then~ to ~n~lyze the logs for tr~ c th~t c~n be removed.  Ensure th~t security groups ~re blocking tr~ c th~t is responsible for high costs.
  B. ;;dd ~n interf~ce VPC endpoint for  Kinesis  D~t~ Stre~ms to the VPC.  Ensure th~t ~pplic~tions h~ve the correct  I;;M permissions to use the interf~ce VPC endpoint.
  C.  En~ble VPC  Flow  Logs ~nd ;;m~zon  Detective.  Review  Detective  ndings for tr~ c th~t is not rel~ted to  Kinesis  D~t~ Stre~ms. Con gure security groups to block th~t tr~ c.
  D. ;;dd ~n interf~ce VPC endpoint for  Kinesis  D~t~ Stre~ms to the VPC.  Ensure th~t the VPC endpoint policy ~llows tr~ c from the ~pplic~tions.

 Correct ;;nswer: D
 D (90%)                                    10%

 Question #116
 ;; ret~il comp~ny h~s ~n on-premises d~t~ center in  Europe. The comp~ny ~lso h~s ~ multi-Region ;;WS presence th~t includes the eu-west-1 ~nd us-e~st-1  Regions. The comp~ny w~nts to be ~ble to route network tr~ c from its on-premises infr~structure into VPCs in either of those  Regions. The comp~ny ~lso needs to support tr~ c th~t is routed directly between VPCs in those  Regions.  No single points of f~ilure c~n exist on the network. The comp~ny ~lre~dy h~s cre~ted two  1 Gbps ;;WS  Direct Connect connections from its on-premises d~t~ center.  E~ch connection goes into ~ sep~r~te  Direct Connect loc~tion in  Europe for high ~v~il~bility. These two loc~tions ~re n~med  DX-;; ~nd  DX-B, respectively.  E~ch  Region h~s ~ single ;;WS Tr~nsit G~tew~y th~t is con gured to route ~ll inter-VPC tr~ c within th~t  Region. Which solution will meet these requirements?
  ;;. Cre~te ~ priv~te VIF from the  DX-;; connection into ~  Direct Connect g~tew~y. Cre~te ~ priv~te VIF from the  DX-B connection into the s~me Direct Connect g~tew~y for high ~v~il~bility. ;;ssoci~te both the eu-west-1 ~nd us-e~st-1 tr~nsit g~tew~ys with the  Direct Connect g~tew~y. Peer the tr~nsit g~tew~ys with e~ch other to support cross-Region routing.
  B. Cre~te ~ tr~nsit VIF from the  DX-;; connection into ~  Direct Connect g~tew~y. ;;ssoci~te the eu-west-1 tr~nsit g~tew~y with this  Direct Connect g~tew~y. Cre~te ~ tr~nsit VIF from the  DX-8 connection into ~ sep~r~te  Direct Connect g~tew~y. ;;ssoci~te the us-e~st-1 tr~nsit g~tew~y with this sep~r~te  Direct Connect g~tew~y.  Peer the  Direct Connect g~tew~ys with e~ch other to support high ~v~il~bility ~nd cross- Region routing.
  C. Cre~te ~ tr~nsit VIF from the  DX-;; connection into ~  Direct Connect g~tew~y. Cre~te ~ tr~nsit VIF from the  DX-B connection into the s~me Direct Connect g~tew~y for high ~v~il~bility. ;;ssoci~te both the eu-west-1 ~nd us-e~st-1 tr~nsit g~tew~ys with this  Direct Connect g~tew~y. Con gure the  Direct Connect g~tew~y to route tr~ c between the tr~nsit g~tew~ys.
  D. Cre~te ~ tr~nsit VIF from the  DX-;; connection into ~  Direct Connect g~tew~y. Cre~te ~ tr~nsit VIF from the  DX-B connection into the s~me Direct Connect g~tew~y for high ~v~il~bility. ;;ssoci~te both the eu-west-1 ~nd us-e~st-1 tr~nsit g~tew~ys with this  Direct Connect g~tew~y. Peer the tr~nsit g~tew~ys with e~ch other to support cross-Region routing.

 Correct ;;nswer: ;;
 D (94%)                                    3%

 Question #117
 ;; comp~ny is running ~n ~pplic~tion in the ;;WS Cloud. The comp~ny's security te~m must ~pprove the cre~tion of ~ll new  I;;M users. When ~ new I;;M user is cre~ted, ~ll ~ccess for the user must be removed ~utom~tic~lly. The security te~m must then receive ~ noti c~tion to ~pprove the user. The comp~ny h~s ~ multi-Region ;;WS CloudTr~il tr~il in the ;;WS ~ccount. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Cre~te ~n ;;m~zon  EventBridge (;;m~zon CloudW~tch  Events) rule.  De ne ~ p~ttern with the det~il-type v~lue set to ;;WS ;;PI C~ll vi~ CloudTr~il ~nd ~n eventN~me of Cre~teUser.
  B. Con gure CloudTr~il to send ~ noti c~tion for the Cre~teUser event to ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic.
  C.  Invoke ~ cont~iner th~t runs in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with ;;WS  F~rg~te technology to remove ~ccess.
  D.  Invoke ~n ;;WS Step  Functions st~te m~chine to remove ~ccess.
  E. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to notify the security te~m.
  F. Use ;;m~zon  Pinpoint to notify the security te~m.

 Correct ;;nswer: ;;DE
 ;;DE (85%)                                   Other

 Question #118
 ;; comp~ny w~nts to migr~te to ;;WS. The comp~ny w~nts to use ~ multi-~ccount structure with centr~lly m~n~ged ~ccess to ~ll ~ccounts ~nd ~pplic~tions. The comp~ny ~lso w~nts to keep the tr~ c on ~ priv~te network.  Multi-f~ctor ~uthentic~tion (MF;;) is required ~t login, ~nd speci c roles ~re ~ssigned to user groups. The comp~ny must cre~te sep~r~te ~ccounts for development. st~ging, production, ~nd sh~red network. The production ~ccount ~nd the sh~red network ~ccount must h~ve connectivity to ~ll ~ccounts. The development ~ccount ~nd the st~ging ~ccount must h~ve ~ccess only to e~ch other. Which combin~tion of steps should ~ solutions ~rchitect t~ke  10 meet these requirements? (Choose three.)
  ;;.  Deploy ~ l~nding zone environment by using ;;WS Control Tower.  Enroll ~ccounts ~nd invite existing ~ccounts into the resulting org~niz~tion in ;;WS Org~niz~tions.
  B.  En~ble ;;WS Security  Hub in ~ll ~ccounts to m~n~ge cross-~ccount ~ccess. Collect  ndings through ;;WS CloudTr~il to force  MF;; login.
  C. Cre~te tr~nsit g~tew~ys ~nd tr~nsit g~tew~y VPC ~tt~chments in e~ch ~ccount. Con gure ~ppropri~te route t~bles.
  D. Set up ~nd en~ble ;;WS  I;;M  Identity Center (;;WS Single Sign-On). Cre~te ~ppropri~te permission sets with required  MF;; for existing ~ccounts.
  E.  En~ble ;;WS Control Tower in ~ll ~ccounts to m~n~ge routing between ~ccounts. Collect  ndings through ;;WS CloudTr~il to force  MF;; login.
  F. Cre~te  I;;M users ~nd groups. Con gure  MF;; for ~ll users. Set up ;;m~zon Cognoto user pools ~nd  Identity pools to m~n~ge ~ccess to ~ccounts ~nd between ~ccounts.

 Correct ;;nswer: BDF
 ;;CD (100%)

 Question #119
 ;; comp~ny runs its ~pplic~tion in the eu-west-1  Region ~nd h~s one ~ccount for e~ch of its environments: development, testing, ~nd production. ;;ll the environments ~re running 24 hours ~ d~y, 7 d~ys ~ week by using st~teful ;;m~zon  EC2 inst~nces ~nd ;;m~zon  RDS for  MySQL d~t~b~ses. The d~t~b~ses ~re between 500 GB ~nd 800 GB in size. The development te~m ~nd testing te~m work on business d~ys during business hours, but the production environment oper~tes 24 hours ~ d~y, 7 d~ys ~ week. The comp~ny w~nts to reduce costs. ;;ll resources ~re t~gged with ~n environment t~g with either development, testing, or production ~s the key. Wh~t should ~ solutions ~rchitect do to reduce costs with the  LE;;ST oper~tion~l effort?
  ;;. Cre~te ~n ;;m~zon  EventBridge rule th~t runs once every d~y. Con gure the rule to invoke one ;;WS  L~mbd~ function th~t st~rts or slops inst~nces b~sed on me t~g, d~y, ~nd time.
  B. Cre~te ~n ;;m~zon  EventBridge rule th~t runs every business d~y in the evening. Con gure the rule to invoke ~n ;;WS  L~mbd~ function th~t stops inst~nces b~sed on the t~g. Cre~te ~ second  EventBridge rule th~t runs every business d~y in the morning. Con gure the second rule lo invoke ~nother  L~mbd~ function th~t st~rts inst~nces b~sed on the t~g.
  C. Cre~te ~n ;;m~zon  EventBridge rule th~t runs every business d~y in the evening, Con gure the rule to invoke ~n ;;WS  L~mbd~ function th~t termin~tes, inst~nces b~sed on the l~g. Cre~te ~ second  EventBridge rule th~t runs every business d~y in the morning. Con gure the second rule lo invoke ~nother  L~mbd~ function th~t restores the inst~nces from their l~st b~ckup b~sed on the t~g.
  D. Cre~te ~n ;;m~zon  EventBridge rule th~t runs every hour. Con gure the rule to invoke one ;;WS  L~mbd~ function th~t termin~tes or restores inst~nces from their l~st b~ckup b~sed on the t~g. d~y, ~nd time.

 Correct ;;nswer: ;;
 B (100%)

 Question #120
 ;; comp~ny is building ~ softw~re-~s-~-service (S~~S) solution on ;;WS. The comp~ny h~s deployed ~n ;;m~zon ;;PI G~tew~y  REST ;;PI with ;;WS L~mbd~ integr~tion in multiple ;;WS  Regions ~nd in the s~me production ~ccount. The comp~ny offers tiered pricing th~t gives customers the ~bility to p~y for the c~p~city to m~ke ~ cert~in number of ;;PI c~lls per second. The premium tier offers up to 3,000 c~lls per second, ~nd customers ~re identi ed by ~ unique ;;PI key. Sever~l premium tier customers in v~rious Regions report th~t they receive error responses of 429 Too  M~ny  Requests from multiple ;;PI methods during pe~k us~ge hours.  Logs indic~te th~t the  L~mbd~ function is never invoked. Wh~t could be the c~use of the error mess~ges for these customers?
  ;;. The  L~mbd~ function re~ched its concurrency limit.
  B. The  L~mbd~ function its  Region limit for concurrency.
  C. The comp~ny re~ched its ;;PI G~tew~y ~ccount limit for c~lls per second.
  D. The comp~ny re~ched its ;;PI G~tew~y def~ult per-method limit for c~lls per second.

 Correct ;;nswer: C
 C (100%)

 Question #121
 ;;  n~nci~l comp~ny is pl~nning to migr~te its web ~pplic~tion from on premises to ;;WS. The comp~ny uses ~ third-p~rty security tool to monitor the inbound tr~ c to the ~pplic~tion. The comp~ny h~s used the security tool for the l~st  15 ye~rs, ~nd the tool h~s no cloud solutions ~v~il~ble from its vendor. The comp~ny's security te~m is concerned ~bout how to integr~te the security tool with ;;WS technology. The comp~ny pl~ns to deploy the ~pplic~tion migr~tion to ;;WS on ;;m~zon  EC2 inst~nces. The  EC2 inst~nces will run in ~n ;;uto Sc~ling group in ~ dedic~ted VPC. The comp~ny needs to use the security tool to inspect ~ll p~ckets th~t come in ~nd out of the VPC. This inspection must occur in re~l time ~nd must not ~ffect the ~pplic~tion's perform~nce. ;; solutions ~rchitect must design ~ t~rget ~rchitecture on ;;WS th~t is highly ~v~il~ble within ~n ;;WS  Region. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;.  Deploy the security tool on  EC2 inst~nces m ~ new ;;uto Sc~ling group in the existing VPC
  B.  Deploy the web ~pplic~tion behind ~  Network  Lo~d  B~l~ncer
  C.  Deploy ~n ;;pplic~tion  Lo~d  B~l~ncer in front of the security tool inst~nces
  D.  Provision ~ G~tew~y  Lo~d  B~l~ncer for e~ch ;;v~il~bility Zone to redirect the tr~ c to the security tool
  E.  Provision ~ tr~nsit g~tew~y to f~cilit~te communic~tion between VPCs.

 Correct ;;nswer: ;;D
 ;;D (54%)                                DE (42%)              2%

 Question #122
 ;; comp~ny h~s purch~sed ~ppli~nces from different vendors. The ~ppli~nces ~ll h~ve  IoT sensors. The sensors send st~tus inform~tion in the vendors' propriet~ry form~ts to ~ leg~cy ~pplic~tion th~t p~rses the inform~tion into JSON. The p~rsing is simple, but e~ch vendor h~s ~ unique form~t. Once d~ily, the ~pplic~tion p~rses ~ll the JSON records ~nd stores the records in ~ rel~tion~l d~t~b~se for ~n~lysis. The comp~ny needs to design ~ new d~t~ ~n~lysis solution th~t c~n deliver f~ster ~nd optimize costs. Which solution will meet these requirements?
  ;;. Connect the  IoT sensors to ;;WS  IoT Core. Set ~ rule to invoke ~n ;;WS  L~mbd~ function to p~rse the inform~tion ~nd s~ve ~ .csv  le to ;;m~zon. S3 Use ;;WS Glue to c~t~log the  les. Use ;;m~zon ;;then~ ~nd ;;m~zon QuickSight for ~n~lysis.
  B.  Migr~te the ~pplic~tion server to ;;WS  F~rg~te, which will receive the inform~tion from  IoT sensors ~nd p~rse the inform~tion into ~ rel~tion~l form~t. S~ve the p~rsed inform~tion to ;;m~zon  Redshlft for ~n~lysis.
  C. Cre~te ~n ;;WS Tr~nsfer for SFTP server. Upd~te the  IoT sensor code to send the inform~tion ~s ~ .csv  le through SFTP to the server. Use ;;WS Glue to c~t~log the  les. Use ;;m~zon ;;then~ for ~n~lysis.
  D. Use ;;WS Snowb~ll  Edge to collect d~t~ from the  IoT sensors directly to perform loc~l ~n~lysis.  Periodic~lly collect the d~t~ into ;;m~zon Redshift to perform glob~l ~n~lysis.

 Correct ;;nswer: C
 ;; (87%)                                   13%

 Question #123
 ;; comp~ny is migr~ting some of its ~pplic~tions to ;;WS. The comp~ny w~nts to migr~te ~nd modernize the ~pplic~tions quickly ~fter it  n~lizes networking ~nd security str~tegies. The comp~ny h~s set up ~n ;;WS  Direct Connect connection in ~ centr~l network ~ccount. The comp~ny expects to h~ve hundreds of ;;WS ~ccounts ~nd VPCs in the ne~r future. The corpor~te network must be ~ble to ~ccess the resources on ;;WS se~mlessly ~nd ~lso must be ~ble to communic~te with ~ll the VPCs. The comp~ny ~lso w~nts to route its cloud resources to the internet through its on-premises d~t~ center. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Cre~te ~  Direct Connect g~tew~y in the centr~l ~ccount.  In e~ch of the ~ccounts, cre~te ~n ~ssoci~tion propos~l by using the  Direct Connect g~tew~y ~nd the ~ccount  ID for every virtu~l priv~te g~tew~y.
  B. Cre~te ~  Direct Connect g~tew~y ~nd ~ tr~nsit g~tew~y in the centr~l network ~ccount. ;;tt~ch the tr~nsit g~tew~y to the  Direct Connect g~tew~y by using ~ tr~nsit VIF.
  C.  Provision ~n internet g~tew~y. ;;tt~ch the internet g~tew~y to subnets. ;;llow internet tr~ c through the g~tew~y.
  D. Sh~re the tr~nsit g~tew~y with other ~ccounts. ;;tt~ch VPCs to the tr~nsit g~tew~y.
  E.  Provision VPC peering ~s necess~ry.
  F.  Provision only priv~te subnets. Open the necess~ry route on the tr~nsit g~tew~y ~nd customer g~tew~y to ~llow outbound internet tr~ c from ;;WS to  ow through  N;;T services th~t run in the d~t~ center.

 Correct ;;nswer: BDF
 BDF (100%)

 Question #124
 ;; comp~ny h~s hundreds of ;;WS ~ccounts. The comp~ny recently implemented ~ centr~lized intern~l process for purch~sing new  Reserved Inst~nces ~nd modifying existing  Reserved  Inst~nces. This process requires ~ll business units th~t w~nt to purch~se or modify  Reserved Inst~nces to submit requests to ~ dedic~ted te~m for procurement.  Previously, business units directly purch~sed or modi ed  Reserved  Inst~nces in their own respective ;;WS ~ccounts ~utonomously. ;; solutions ~rchitect needs to enforce the new process in the most secure w~y possible. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;.  Ensure th~t ~ll ;;WS ~ccounts ~re p~rt of ~n org~niz~tion in ;;WS Org~niz~tions with ~ll fe~tures en~bled.
  B. Use ;;WS Con g to report on the ~tt~chment of ~n  I;;M policy th~t denies ~ccess to the ec2:Purch~seReservedInst~ncesOffering ~ction ~nd the ec2:ModifyReservedInst~nces ~ction.
  C.  In e~ch ;;WS ~ccount, cre~te ~n  I;;M policy th~t denies the ec2:Purch~seReservedInst~ncesOffering ~ction ~nd the ec2:ModifyReservedInst~nces ~ction.
  D. Cre~te ~n SCP th~t denies the ec2:Purch~seReservedInst~ncesOffering ~ction ~nd the ec2:ModifyReservedInst~nces ~ction. ;;tt~ch the SCP to e~ch OU of the org~niz~tion.
  E.  Ensure th~t ~ll ;;WS ~ccounts ~re p~rt of ~n org~niz~tion in ;;WS Org~niz~tions th~t uses the consolid~ted billing fe~ture.

 Correct ;;nswer: ;;D
 ;;D (100%)

 Question #125
 ;; comp~ny is running ~ critic~l ~pplic~tion th~t uses ~n ;;m~zon  RDS for  MySQL d~t~b~se to store d~t~. The  RDS  DB inst~nce is deployed in  Multi- ;;Z mode. ;; recent  RDS d~t~b~se f~ilover test c~used ~ 40-second out~ge to the ~pplic~tion. ;; solutions ~rchitect needs to design ~ solution to reduce the out~ge time to less th~n 20 seconds. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose three.)
  ;;. Use ;;m~zon  El~stiC~che for  Memc~ched in front of the d~t~b~se
  B. Use ;;m~zon  El~stiC~che for  Redis in front of the d~t~b~se
  C. Use  RDS  Proxy in front of the d~t~b~se.
  D.  Migr~te the d~t~b~se to ;;m~zon ;;uror~  MySQL.
  E. Cre~te ~n ;;m~zon ;;uror~  Replic~.
  F. Cre~te ~n  RDS for  MySQL re~d replic~

 Correct ;;nswer: BCF
 CDE (91%)                                   9%

 Question #126
 ;;n ;;WS p~rtner comp~ny is building ~ service in ;;WS Org~niz~tions using its org~niz~tion n~med org1. This service requires the p~rtner comp~ny to h~ve ~ccess to ;;WS resources in ~ customer ~ccount, which is in ~ sep~r~te org~niz~tion n~med org2. The comp~ny must est~blish le~st privilege security ~ccess using ~n ;;PI or comm~nd line tool to the customer ~ccount. Wh~t is the  MOST secure w~y to ~llow org1 to ~ccess resources in org2?
  ;;. The customer should provide the p~rtner comp~ny with their ;;WS ~ccount ~ccess keys to log in ~nd perform the required t~sks.
  B. The customer should cre~te ~n  I;;M user ~nd ~ssign the required permissions to the  I;;M user. The customer should then provide the credenti~ls to the p~rtner comp~ny to log in ~nd perform the required t~sks.
  C. The customer should cre~te ~n  I;;M role ~nd ~ssign the required permissions to the  I;;M role. The p~rtner comp~ny should then use the I;;M role’s ;;m~zon  Resource  N~me (;;RN) when requesting ~ccess to perform the required t~sks.
  D. The customer should cre~te ~n  I;;M role ~nd ~ssign the required permissions to the  I;;M role. The p~rtner comp~ny should then use the  I;;M role’s ;;m~zon  Resource  N~me (;;RN), including the extern~l  ID in the  I;;M role’s trust policy, when requesting ~ccess to perform the required t~sks.

 Correct ;;nswer: D
 D (100%)

 Question #127
 ;; delivery comp~ny needs to migr~te its third-p~rty route pl~nning ~pplic~tion to ;;WS. The third p~rty supplies ~ supported  Docker im~ge from ~ public registry. The im~ge c~n run in ~s m~ny cont~iners ~s required to gener~te the route m~p. The comp~ny h~s divided the delivery ~re~ into sections with supply hubs so th~t delivery drivers tr~vel the shortest dist~nce possible from the hubs to the customers. To reduce the time necess~ry to gener~te route m~ps, e~ch section uses its own set of  Docker cont~iners with ~ custom con gur~tion th~t processes orders only in the section's ~re~. The comp~ny needs the ~bility to ~lloc~te resources cost-effectively b~sed on the number of running cont~iners. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster on ;;m~zon  EC2. Use the ;;m~zon  EKS CLI to l~unch the pl~nning ~pplic~tion in pods by using the --t~gs option to ~ssign ~ custom t~g to the pod.
  B. Cre~te ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster on ;;WS  F~rg~te. Use the ;;m~zon  EKS CLI to l~unch the pl~nning ~pplic~tion. Use the ;;WS CLI t~g-resource ;;PI c~ll to ~ssign ~ custom t~g to the pod.
  C. Cre~te ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster on ;;m~zon  EC2. Use the ;;WS CLI with run-t~sks set to true to l~unch the pl~nning ~pplic~tion by using the --t~gs option to ~ssign ~ custom t~g to the t~sk.
  D. Cre~te ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster on ;;WS  F~rg~te. Use the ;;WS CLI run-t~sk comm~nd ~nd set en~bleECSM~n~gedT~gs to true to l~unch the pl~nning ~pplic~tion. Use the --t~gs option to ~ssign ~ custom t~g to the t~sk.

 Correct ;;nswer: D
 D (82%)                                   B (18%)

 Question #128
 ;; softw~re comp~ny hosts ~n ~pplic~tion on ;;WS with resources in multiple ;;WS ~ccounts ~nd  Regions. The ~pplic~tion runs on ~ group of ;;m~zon  EC2 inst~nces in ~n ~pplic~tion VPC loc~ted in the us-e~st-1  Region with ~n  IPv4 CIDR block of  10.10.0.0/16.  In ~ different ;;WS ~ccount, ~ sh~red services VPC is loc~ted in the us-e~st-2  Region with ~n  IPv4 CIDR block of  10.10.10.0/24. When ~ cloud engineer uses ;;WS CloudForm~tion to ~ttempt to peer the ~pplic~tion VPC with the sh~red services VPC, ~n error mess~ge indic~tes ~ peering f~ilure. Which f~ctors could c~use this error? (Choose two.)
  ;;. The  IPv4 CIDR r~nges of the two VPCs overl~p
  B. The VPCs ~re not in the s~me  Region
  C. One or both ~ccounts do not h~ve ~ccess to ~n  Internet g~tew~y
  D. One of the VPCs w~s not sh~red through ;;WS  Resource ;;ccess  M~n~ger
  E. The  I;;M role in the peer ~ccepter ~ccount does not h~ve the correct permissions

 Correct ;;nswer: ;;E
 ;;E (86%)                                    14%

 Question #129
 ;;n extern~l ~udit of ~ comp~ny’s serverless ~pplic~tion reve~ls  I;;M policies th~t gr~nt too m~ny permissions. These policies ~re ~tt~ched to the comp~ny's ;;WS  L~mbd~ execution roles.  Hundreds of the comp~ny's  L~mbd~ functions h~ve bro~d ~ccess permissions such ~s full ~ccess to ;;m~zon S3 buckets ~nd ;;m~zon  Dyn~moDB t~bles. The comp~ny w~nts e~ch function to h~ve only the minimum permissions th~t the function needs to complete its t~sk. ;; solutions ~rchitect must determine which permissions e~ch  L~mbd~ function needs. Wh~t should the solutions ~rchitect do to meet this requirement with the  LE;;ST ~mount of effort?
  ;;. Set up ;;m~zon CodeGuru to pro le the  L~mbd~ functions ~nd se~rch for ;;WS ;;PI c~lls. Cre~te ~n inventory of the required ;;PI c~lls ~nd resources for e~ch  L~mbd~ function. Cre~te new  I;;M ~ccess policies for e~ch  L~mbd~ function.  Review the new policies to ensure th~t they meet the comp~ny's business requirements.
  B. Turn on ;;WS CloudTr~il logging for the ;;WS ~ccount. Use ;;WS  Identity ~nd ;;ccess  M~n~gement ;;ccess ;;n~lyzer to gener~te  I;;M ~ccess policies b~sed on the ~ctivity recorded in the CloudTr~il log.  Review the gener~ted policies to ensure th~t they meet the comp~ny's business requirements.
  C. Turn on ;;WS CloudTr~il logging for the ;;WS ~ccount. Cre~te ~ script to p~rse the CloudTr~il log, se~rch for ;;WS ;;PI c~lls by  L~mbd~ execution role, ~nd cre~te ~ summ~ry report.  Review the report. Cre~te  I;;M ~ccess policies th~t provide more restrictive permissions for e~ch L~mbd~ function.
  D. Turn on ;;WS CloudTr~il logging for the ;;WS ~ccount.  Export the CloudTr~il logs to ;;m~zon S3. Use ;;m~zon  EMR to process the CloudTr~il logs in ;;m~zon S3 ~nd produce ~ report of ;;PI c~lls ~nd resources used by e~ch execution role. Cre~te ~ new  I;;M ~ccess policy for e~ch role.  Export the gener~ted roles to ~n S3 bucket.  Review the gener~ted policies to ensure th~t they meet the comp~ny’s business requirements.

 Correct ;;nswer: B
 B (100%)

 Question #130
 ;; solutions ~rchitect must ~n~lyze ~ comp~ny’s ;;m~zon  EC2 inst~nces ~nd ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes to determine whether the comp~ny is using resources e ciently. The comp~ny is running sever~l l~rge, high-memory  EC2 inst~nces to host d~t~b~se clusters th~t ~re deployed in ~ctive/p~ssive con gur~tions. The utiliz~tion of these  EC2 inst~nces v~ries by the ~pplic~tions th~t use the d~t~b~ses, ~nd the comp~ny h~s not identi ed ~ p~ttern. The solutions ~rchitect must ~n~lyze the environment ~nd t~ke ~ction b~sed on the  ndings. Which solution meets these requirements  MOST cost-effectively?
  ;;. Cre~te ~ d~shbo~rd by using ;;WS Systems  M~n~ger OpsCenter. Con gure visu~liz~tions for ;;m~zon CloudW~tch metrics th~t ~re ~ssoci~ted with the  EC2 inst~nces ~nd their  EBS volumes.  Review the d~shbo~rd periodic~lly, ~nd identify us~ge p~tterns.  Rightsize the  EC2 inst~nces b~sed on the pe~ks in the metrics.
  B. Turn on ;;m~zon CloudW~tch det~iled monitoring for the  EC2 inst~nces ~nd their  EBS volumes. Cre~te ~nd review ~ d~shbo~rd th~t is b~sed on the metrics.  Identify us~ge p~tterns.  Rightsize the  EC2 inst~nces b~sed on the pe~ks in the metrics.
  C.  Inst~ll the ;;m~zon CloudW~tch ~gent on e~ch of the  EC2 inst~nces. Turn on ;;WS Compute Optimizer, ~nd let it run for ~t le~st  12 hours. Review the recommend~tions from Compute Optimizer, ~nd rightsize the  EC2 inst~nces ~s directed.
  D. Sign up for the ;;WS  Enterprise Support pl~n. Turn on ;;WS Trusted ;;dvisor. W~it  12 hours.  Review the recommend~tions from Trusted ;;dvisor, ~nd rightsize the  EC2 inst~nces ~s directed.

 Correct ;;nswer: C
 C (95%)                                   5%

 Question #131
 ;; comp~ny uses ;;WS Org~niz~tions for ~ multi-~ccount setup in the ;;WS Cloud. The comp~ny uses ;;WS Control Tower for govern~nce ~nd uses ;;WS Tr~nsit G~tew~y for VPC connectivity ~cross ~ccounts. In ~n ;;WS ~pplic~tion ~ccount, the comp~ny’s ~pplic~tion te~m h~s deployed ~ web ~pplic~tion th~t uses ;;WS  L~mbd~ ~nd ;;m~zon  RDS. The comp~ny's d~t~b~se ~dministr~tors h~ve ~ sep~r~te  DB;; ~ccount ~nd use the ~ccount to centr~lly m~n~ge ~ll the d~t~b~ses ~cross the org~niz~tion. The d~t~b~se ~dministr~tors use ~n ;;m~zon  EC2 inst~nce th~t is deployed in the  DB;; ~ccount to ~ccess ~n  RDS d~t~b~se th~t is deployed m the ~pplic~tion ~ccount. The ~pplic~tion te~m h~s stored the d~t~b~se credenti~ls ~s secrets in ;;WS Secrets  M~n~ger in the ~pplic~tion ~ccount. The ~pplic~tion te~m is m~nu~lly sh~ring the secrets with the d~t~b~se ~dministr~tors. The secrets ~re encrypted by the def~ult ;;WS m~n~ged key for Secrets  M~n~ger in the ~pplic~tion ~ccount. ;; solutions ~rchitect needs to implement ~ solution th~t gives the d~t~b~se ~dministr~tors ~ccess to the d~t~b~se ~nd elimin~tes the need to m~nu~lly sh~re the secrets. Which solution will meet these requirements?
  ;;. Use ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M) to sh~re the secrets from the ~pplic~tion ~ccount with the  DB;; ~ccount.  In the  DB;; ~ccount, cre~te ~n  I;;M role th~t is n~med  DB;;-;;dmin. Gr~nt the role the required permissions to ~ccess the sh~red secrets. ;;tt~ch the  DB;;- ;;dmin role to the  EC2 inst~nce for ~ccess to the cross-~ccount secrets.
  B.  In the ~pplic~tion ~ccount, cre~te ~n  I;;M role th~t is n~med  DB;;-Secret. Gr~nt the role the required permissions to ~ccess the secrets.  In the  DB;; ~ccount, cre~te ~n  I;;M role th~t is n~med  DB;;-;;dmin. Gr~nt the  DB;;-;;dmin role the required permissions to ~ssume the  DB;;-Secret role in the ~pplic~tion ~ccount. ;;tt~ch the  DB;;-;;dmin role to the  EC2 inst~nce for ~ccess to the cross-~ccount secrets
  C.  In the  DB;; ~ccount cre~te ~n  I;;M role th~t is n~med  DB;;-;;dmin. Gr~nt the role the required permissions to ~ccess the secrets ~nd the def~ult ;;WS m~n~ged key in the ~pplic~tion ~ccount.  In the ~pplic~tion ~ccount, ~tt~ch resource-b~sed policies to the key to ~llow ~ccess from the  DB;; ~ccount. ;;tt~ch the  DB;;-;;dmin role to the  EC2 inst~nce for ~ccess to the cross-~ccount secrets.
  D.  In the  DB;; ~ccount, cre~te ~n  I;;M role th~t is n~med  DB;;-;;dmin. Gr~nt the role the required permissions to ~ccess the secrets in the ~pplic~tion ~ccount. ;;tt~ch ~n SCP to the ~pplic~tion ~ccount to ~llow ~ccess to the secrets from the  DB;; ~ccount. ;;tt~ch the  DB;;-;;dmin role to the  EC2 inst~nce for ~ccess to the cross-~ccount secrets.

 Correct ;;nswer: ;;
 B (80%)                               8%      8%

 Question #132
 ;; comp~ny m~n~ges multiple ;;WS ~ccounts by using ;;WS Org~niz~tions. Under the root OU, the comp~ny h~s two OUs:  Rese~rch ~nd  D~t~Ops. Bec~use of regul~tory requirements, ~ll resources th~t the comp~ny deploys in the org~niz~tion must reside in the ~p-northe~st-1  Region. ;;ddition~lly,  EC2 inst~nces th~t the comp~ny deploys in the  D~t~Ops OU must use ~ prede ned list of inst~nce types. ;; solutions ~rchitect must implement ~ solution th~t ~pplies these restrictions. The solution must m~ximize oper~tion~l e ciency ~nd must minimize ongoing m~inten~nce. Which combin~tion of steps will meet these requirements? (Choose two.)
  ;;. Cre~te ~n  I;;M role in one ~ccount under the  D~t~Ops OU. Use the ec2:Inst~nceType condition key in ~n inline policy on the role to restrict ~ccess to speci c inst~nce type.
  B. Cre~te ~n  I;;M user in ~ll ~ccounts under the root OU. Use the ~ws:RequestedRegion condition key in ~n inline policy on e~ch user to restrict ~ccess to ~ll ;;WS  Regions except ~p-northe~st-1.
  C. Cre~te ~n SCP. Use the ~ws:RequestedRegion condition key to restrict ~ccess to ~ll ;;WS  Regions except ~p-northe~st-1. ;;pply the SCP to the root OU.
  D. Cre~te ~n SCP. Use the ec2:Region condition key to restrict ~ccess to ~ll ;;WS  Regions except ~p-northe~st-1. ;;pply the SCP to the root OU, the  D~t~Ops OU, ~nd the  Rese~rch OU.
  E. Cre~te ~n SCP. Use the ec2:Inst~nceType condition key to restrict ~ccess to speci c inst~nce types. ;;pply the SCP to the  D~t~Ops OU.

 Correct ;;nswer: CE
 CE (100%)

 Question #133
 ;; comp~ny runs ~ serverless ~pplic~tion in ~ single ;;WS  Region. The ~pplic~tion ~ccesses extern~l URLs ~nd extr~cts met~d~t~ from those sites. The comp~ny uses ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic to publish URLs to ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. ;;n ;;WS  L~mbd~ function uses the queue ~s ~n event source ~nd processes the URLs from the queue.  Results ~re s~ved to ~n ;;m~zon S3 bucket. The comp~ny w~nts to process e~ch URL in other  Regions to comp~re possible differences in site loc~liz~tion. URLs must be published from the existing  Region.  Results must be written to the existing S3 bucket in the current  Region. Which combin~tion of ch~nges will produce multi-Region deployment th~t meets these requirements? (Choose two.)
  ;;.  Deploy the SQS queue with the  L~mbd~ function to other  Regions.
  B. Subscribe the SNS topic in e~ch  Region to the SQS queue.
  C. Subscribe the SQS queue in e~ch  Region to the SNS topic.
  D. Con gure the SQS queue to publish URLs to SNS topics in e~ch  Region.
  E.  Deploy the SNS topic ~nd the  L~mbd~ function to other  Regions.

 Correct ;;nswer: ;;C
 ;;C (100%)

 Question #134
 ;; comp~ny runs ~ propriet~ry st~teless  ETL ~pplic~tion on ~n ;;m~zon  EC2  Linux inst~nces. The ~pplic~tion is ~  Linux bin~ry, ~nd the source code c~nnot be modi ed. The ~pplic~tion is single-thre~ded, uses 2 GB of  R;;M, ~nd is highly CPU intensive. The ~pplic~tion is scheduled to run every 4 hours ~nd runs for up to 20 minutes. ;; solutions ~rchitect w~nts to revise the ~rchitecture for the solution. Which str~tegy should the solutions ~rchitect use?
  ;;. Use ;;WS  L~mbd~ to run the ~pplic~tion. Use ;;m~zon CloudW~tch  Logs to invoke the  L~mbd~ function every 4 hours.
  B. Use ;;WS  B~tch to run the ~pplic~tion. Use ~n ;;WS Step  Functions st~te m~chine to invoke the ;;WS  B~tch job every 4 hours.
  C. Use ;;WS  F~rg~te to run the ~pplic~tion. Use ;;m~zon  EventBridge (;;m~zon CloudW~tch  Events) to invoke the  F~rg~te t~sk every 4 hours.
  D. Use ;;m~zon  EC2 Spot  Inst~nces to run the ~pplic~tion. Use ;;WS CodeDeploy to deploy ~nd run the ~pplic~tion every 4 hours.

 Correct ;;nswer: C
 C (88%)                                    13%

 Question #135
 ;; comp~ny is cre~ting ~ sequel for ~ popul~r online g~me. ;; l~rge number of users from ~ll over the world will pl~y the g~me within the  rst week ~fter l~unch. Currently, the g~me consists of the following components deployed in ~ single ;;WS  Region: • ;;m~zon S3 bucket th~t stores g~me ~ssets • ;;m~zon  Dyn~moDB t~ble th~t stores pl~yer scores ;; solutions ~rchitect needs to design ~ multi-Region solution th~t will reduce l~tency, improve reli~bility, ~nd require the le~st effort to implement. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Cre~te ~n ;;m~zon CloudFront distribution to serve ~ssets from the S3 bucket. Con gure S3 Cross-Region  Replic~tion. Cre~te ~ new Dyn~moDB t~ble in ~ new  Region. Use the new t~ble ~s ~ replic~ t~rget for  Dyn~moDB glob~l t~bles.
  B. Cre~te ~n ;;m~zon CloudFront distribution to serve ~ssets from the S3 bucket. Con gure S3 S~me-Region  Replic~tion. Cre~te ~ new Dyn~moDB t~ble in ~ new  Region. Con gure ~synchronous replic~tion between the  Dyn~moDB t~bles by using ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) with ch~nge d~t~ c~pture (CDC).
  C. Cre~te ~nother S3 bucket in ~ new  Region, ~nd con gure S3 Cross-Region  Replic~tion between the buckets. Cre~te ~n ;;m~zon CloudFront distribution ~nd con gure origin f~ilover with two origins ~ccessing the S3 buckets in e~ch  Region. Con gure  Dyn~moDB glob~l t~bles by en~bling ;;m~zon  Dyn~moDB Stre~ms, ~nd ~dd ~ replic~ t~ble in ~ new  Region.
  D. Cre~te ~nother S3 bucket in the sine  Region, ~nd con gure S3 S~me-Region  Replic~tion between the buckets. Cre~te ~n ;;m~zon CloudFront distribution ~nd con gure origin f~ilover with two origins ~ccessing the S3 buckets. Cre~te ~ new  Dyn~moDB t~ble in ~ new  Region. Use the new t~ble ~s ~ replic~ t~rget for  Dyn~moDB glob~l t~bles.

 Correct ;;nswer: C
 C (86%)                                    14%

 Question #136
 ;; comp~ny h~s ~n on-premises website ~pplic~tion th~t provides re~l est~te inform~tion for potenti~l renters ~nd buyers. The website uses ~ J~v~ b~ckend ~nd ~  NoSQL  MongoDB d~t~b~se to store subscriber d~t~. The comp~ny needs to migr~te the entire ~pplic~tion to ;;WS with ~ simil~r structure. The ~pplic~tion must be deployed for high ~v~il~bility, ~nd the comp~ny c~nnot m~ke ch~nges to the ~pplic~tion. Which solution will meet these requirements?
  ;;. Use ~n ;;m~zon ;;uror~  DB cluster ~s the d~t~b~se for the subscriber d~t~.  Deploy ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group ~cross multiple ;;v~il~bility Zones for the J~v~ b~ckend ~pplic~tion.
  B. Use  MongoDB on ;;m~zon  EC2 inst~nces ~s the d~t~b~se for the subscriber d~t~.  Deploy  EC2 inst~nces in ~n ;;uto Sc~ling group in ~ single ;;v~il~bility Zone for the J~v~ b~ckend ~pplic~tion.
  C. Con gure ;;m~zon  DocumentDB (with  MongoDB comp~tibility) with ~ppropri~tely sized inst~nces in multiple ;;v~il~bility Zones ~s the d~t~b~se for the subscriber d~t~.  Deploy ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group ~cross multiple ;;v~il~bility Zones for the J~v~ b~ckend ~pplic~tion.
  D. Con gure ;;m~zon  DocumentDB (with  MongoDB comp~tibility) in on-dem~nd c~p~city mode in multiple ;;v~il~bility Zones ~s the d~t~b~se for the subscriber d~t~.  Deploy ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group ~cross multiple ;;v~il~bility Zones for the J~v~ b~ckend ~pplic~tion.

 Correct ;;nswer: D
 C (87%)                                   13%

 Question #137
 ;; digit~l m~rketing comp~ny h~s multiple ;;WS ~ccounts th~t belong to v~rious te~ms. The cre~tive te~m uses ~n ;;m~zon S3 bucket in its ;;WS ~ccount to securely store im~ges ~nd medi~  les th~t ~re used ~s content for the comp~ny’s m~rketing c~mp~igns. The cre~tive te~m w~nts to sh~re the S3 bucket with the str~tegy te~m so th~t the str~tegy te~m c~n view the objects. ;; solutions ~rchitect h~s cre~ted ~n  I;;M role th~t is n~med str~tegy_reviewer in the Str~tegy ~ccount. The solutions ~rchitect ~lso h~s set up ~ custom ;;WS  Key  M~n~gement Service (;;WS  KMS) key in the Cre~tive ~ccount ~nd h~s ~ssoci~ted the key with the S3 bucket.  However, when users from the Str~tegy ~ccount ~ssume the  I;;M role ~nd try to ~ccess objects in the S3 bucket, they receive ~n ;;ccess  Denied error. The solutions ~rchitect must ensure th~t users in the Str~tegy ~ccount c~n ~ccess the S3 bucket. The solution must provide these users with only the minimum permissions th~t they need. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose three.)
  ;;. Cre~te ~ bucket policy th~t includes re~d permissions for the S3 bucket. Set the princip~l of the bucket policy to the ~ccount  ID of the Str~tegy ~ccount.
  B. Upd~te the str~tegy_reviewer  I;;M role to gr~nt full permissions for the S3 bucket ~nd to gr~nt decrypt permissions for the custom  KMS key.
  C. Upd~te the custom  KMS key policy in the Cre~tive ~ccount to gr~nt decrypt permissions to the str~tegy_reviewer  I;;M role.
  D. Cre~te ~ bucket policy th~t includes re~d permissions for the S3 bucket. Set the princip~l of the bucket policy to ~n ~nonymous user.
  E. Upd~te the custom  KMS key policy in the Cre~tive ~ccount to gr~nt encrypt permissions to the str~tegy_reviewer  I;;M role.
  F. Upd~te the str~tegy_reviewer  I;;M role to gr~nt re~d permissions for the S3 bucket ~nd to gr~nt decrypt permissions for the custom  KMS key.

 Correct ;;nswer: BCF
 ;;CF (100%)

 Question #138
 ;; life sciences comp~ny is using ~ combin~tion of open source tools to m~n~ge d~t~ ~n~lysis work ows ~nd  Docker cont~iners running on servers in its on-premises d~t~ center to process genomics d~t~. Sequencing d~t~ is gener~ted ~nd stored on ~ loc~l stor~ge ~re~ network (S;;N), ~nd then the d~t~ is processed. The rese~rch ~nd development te~ms ~re running into c~p~city issues ~nd h~ve decided to re-~rchitect their genomics ~n~lysis pl~tform on ;;WS to sc~le b~sed on worklo~d dem~nds ~nd reduce the turn~round time from weeks to d~ys. The comp~ny h~s ~ high-speed ;;WS  Direct Connect connection. Sequencers will gener~te ~round 200 GB of d~t~ for e~ch genome, ~nd individu~l jobs c~n t~ke sever~l hours to process the d~t~ with ide~l compute c~p~city. The end result will be stored in ;;m~zon S3. The comp~ny is expecting  10-15 job requests e~ch d~y. Which solution meets these requirements?
  ;;. Use regul~rly scheduled ;;WS Snowb~ll  Edge devices to tr~nsfer the sequencing d~t~ into ;;WS. When ;;WS receives the Snowb~ll  Edge device ~nd the d~t~ is lo~ded into ;;m~zon S3, use S3 events to trigger ~n ;;WS  L~mbd~ function to process the d~t~.
  B. Use ;;WS  D~t~  Pipeline to tr~nsfer the sequencing d~t~ to ;;m~zon S3. Use S3 events to trigger ~n ;;m~zon  EC2 ;;uto Sc~ling group to l~unch custom-;;MI  EC2 inst~nces running the  Docker cont~iners to process the d~t~.
  C. Use ;;WS  D~t~Sync to tr~nsfer the sequencing d~t~ to ;;m~zon S3. Use S3 events to trigger ~n ;;WS  L~mbd~ function th~t st~rts ~n ;;WS Step  Functions work ow. Store the  Docker im~ges in ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR) ~nd trigger ;;WS  B~tch to run the cont~iner ~nd process the sequencing d~t~.
  D. Use ~n ;;WS Stor~ge G~tew~y  le g~tew~y to tr~nsfer the sequencing d~t~ to ;;m~zon S3. Use S3 events to trigger ~n ;;WS  B~tch job th~t executes on ;;m~zon  EC2 inst~nces running the  Docker cont~iners to process the d~t~.

 Correct ;;nswer: C
 C (72%)                                 D (28%)

 Question #139
 ;; comp~ny runs ~ content m~n~gement ~pplic~tion on ~ single Windows ;;m~zon  EC2 inst~nce in ~ development environment. The ~pplic~tion re~ds ~nd writes st~tic content to ~ 2 TB ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume th~t is ~tt~ched to the inst~nce ~s the root device. The comp~ny pl~ns to deploy this ~pplic~tion in production ~s ~ highly ~v~il~ble ~nd f~ult-toler~nt solution th~t runs on ~t le~st three  EC2 inst~nces ~cross multiple ;;v~il~bility Zones. ;; solutions ~rchitect must design ~ solution th~t joins ~ll the inst~nces th~t run the ~pplic~tion to ~n ;;ctive  Directory dom~in. The solution ~lso must implement Windows ;;CLs to control ~ccess to  le contents. The ~pplic~tion ~lw~ys must m~int~in ex~ctly the s~me content on ~ll running inst~nces ~t ~ny given point in time. Which solution will meet these requirements with the  LE;;ST m~n~gement overhe~d?
  ;;. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le sh~re. Cre~te ~n ;;uto Sc~ling group th~t extends ~cross three ;;v~il~bility Zones ~nd m~int~ins ~ minimum size of three inst~nces.  Implement ~ user d~t~ script to inst~ll the ~pplic~tion, join the inst~nce to the ;;D dom~in, ~nd mount the  EFS  le sh~re.
  B. Cre~te ~ new ;;MI from the current  EC2  Inst~nce th~t is running. Cre~te ~n ;;m~zon  FSx for  Lustre  le system. Cre~te ~n ;;uto Sc~ling group th~t extends ~cross three ;;v~il~bility Zones ~nd m~int~ins ~ minimum size of three inst~nces.  Implement ~ user d~t~ script to join the inst~nce to the ;;D dom~in ~nd mount the  FSx for  Lustre  le system.
  C. Cre~te ~n ;;m~zon  FSx for Windows  File Server  le system. Cre~te ~n ;;uto Sc~ling group th~t extends ~cross three ;;v~il~bility Zones ~nd m~int~ins ~ minimum size of three inst~nces.  Implement ~ user d~t~ script to inst~ll the ~pplic~tion ~nd mount the  FSx for Windows  File Server  le system.  Perform ~ se~mless dom~in join to join the inst~nce to the ;;D dom~in.
  D. Cre~te ~ new ;;MI from the current  EC2 inst~nce th~t is running. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system. Cre~te ~n ;;uto Sc~ling group th~t extends ~cross three ;;v~il~bility Zones ~nd m~int~ins ~ minimum size of three  Inst~nces.  Perform ~ se~mless dom~in join to join the inst~nce to the ;;D dom~in.

 Correct ;;nswer: B
 C (94%)                                    6%

 Question #140
 ;; softw~re ~s ~ service (S~~S) b~sed comp~ny provides ~ c~se m~n~gement solution to customers ;;3 p~rt of the solution. The comp~ny uses ~ st~nd~lone Simple  M~il Tr~nsfer  Protocol (SMTP) server to send em~il mess~ges from ~n ~pplic~tion. The ~pplic~tion ~lso stores ~n em~il templ~te for ~cknowledgement em~il mess~ges th~t popul~te customer d~t~ before the ~pplic~tion sends the em~il mess~ge to the customer. The comp~ny pl~ns to migr~te this mess~ging function~lity to the ;;WS Cloud ~nd needs to minimize oper~tion~l overhe~d. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Set up ~n SMTP server on ;;m~zon  EC2 inst~nces by using ~n ;;MI from the ;;WS  M~rketpl~ce. Store the em~il templ~te in ~n ;;m~zon S3 bucket. Cre~te ~n ;;WS  L~mbd~ function to retrieve the templ~te from the S3 bucket ~nd to merge the customer d~t~ from the ~pplic~tion with the templ~te. Use ~n SDK in the  L~mbd~ function to send the em~il mess~ge.
  B. Set up ;;m~zon Simple  Em~il Service (;;m~zon SES) to send em~il mess~ges. Store the em~il templ~te in ~n ;;m~zon S3 bucket. Cre~te ~n ;;WS  L~mbd~ function to retrieve the templ~te from the S3 bucket ~nd to merge the customer d~t~ from the ~pplic~tion with the templ~te. Use ~n SDK in the  L~mbd~ function to send the em~il mess~ge.
  C. Set up ~n SMTP server on ;;m~zon  EC2 inst~nces by using ~n ;;MI from the ;;WS  M~rketpl~ce. Store the em~il templ~te in ;;m~zon Simple Em~il Service (;;m~zon SES) with p~r~meters for the customer d~t~. Cre~te ~n ;;WS  L~mbd~ function to c~ll the SES templ~te ~nd to p~ss customer d~t~ to repl~ce the p~r~meters. Use the ;;WS  M~rketpl~ce SMTP server to send the em~il mess~ge.
  D. Set up ;;m~zon Simple  Em~il Service (;;m~zon SES) to send em~il mess~ges. Store the em~il templ~te on ;;m~zon SES with p~r~meters for the customer d~t~. Cre~te ~n ;;WS  L~mbd~ function to c~ll the SendTempl~tedEm~il ;;PI oper~tion ~nd to p~ss customer d~t~ to repl~ce the p~r~meters ~nd the em~il destin~tion.

 Correct ;;nswer: B
 D (96%)                                   4%

 Question #141
 ;; comp~ny is processing videos in the ;;WS Cloud by Using ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group.  It t~kes 30 minutes to process ~ video Sever~l  EC2 inst~nces sc~le in ~nd out depending on the number of videos in ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. The comp~ny h~s con gured the SQS queue with ~ redrive policy th~t speci es ~ t~rget de~d-letter queue ~nd ~ m~xReceiveCount of  1. The comp~ny h~s set the visibility timeout for the SQS queue to  1 hour. The comp~ny h~s set up ~n ;;m~zon CloudW~tch ~l~rm to notify the development te~m when there ~re mess~ges in the de~d-letter queue. Sever~l times during the d~y. the development te~m receives noti c~tion th~t mess~ges ~re in the de~d-letter queue ~nd th~t videos h~ve not been processed property. ;;n investig~tion  nds no errors m the ~pplic~tion logs. How c~n the comp~ny solve this problem?
  ;;. Turn on termin~tion protection tor the  EC2  Inst~nces
  B. Upd~te the visibility timeout for the SQS queue to 3 hours
  C. Con gure sc~le-in protection for the inst~nces during processing
  D. Upd~te the redrive policy ~nd set m~xReceiveCount to 0.

 Correct ;;nswer: D
 C (78%)                                D (17%)   4%

 Question #142
 ;; comp~ny h~s developed ;;PIs th~t use ;;m~zon ;;PI G~tew~y with  Region~l endpoints. The ;;PIs c~ll ;;WS  L~mbd~ functions th~t use ;;PI G~tew~y ~uthentic~tion mech~nisms. ;;fter ~ design review, ~ solutions ~rchitect identi es ~ set of ;;PIs th~t do not require public ~ccess. The solutions ~rchitect must design ~ solution to m~ke the set of ;;PIs ~ccessible only from ~ VPC. ;;ll ;;PIs need to be c~lled with ~n ~uthentic~ted user Which solution will meet these requirements with the  LE;;ST ~mount of effort?
  ;;. Cre~te ~n intern~l ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Cre~te ~ t~rget group. Select the  L~mbd~ function to c~ll. Use the ;;LB  DNS n~me to c~ll the ;;PI from the VPC.
  B.  Remove the  DNS entry th~t is ~ssoci~ted with the ;;PI in ;;PI G~tew~y. Cre~te ~ hosted zone in ;;m~zon  Route 53. Cre~te ~ CN;;ME record in the hosted zone. Upd~te the ;;PI in ;;PI G~tew~y with the CN;;ME record. Use the CN;;ME record to c~ll the ;;PI from the VPC.
  C. Upd~te the ;;PI endpoint from  Region~l to priv~te in ;;PI G~tew~y. Cre~te ~n interf~ce VPC endpoint in the VPCre~te ~ resource policy, ~nd ~tt~ch it to the ;;PI. Use the VPC endpoint to c~ll the ;;PI from the VPC.
  D.  Deploy the  L~mbd~ functions inside the VPC  Provision ~n  EC2 inst~nce, ~nd inst~ll ~n ;;p~che server.  From the ;;p~che server, c~ll the L~mbd~ functions. Use the intern~l CN;;ME record of the  EC2 inst~nce to c~ll the ;;PI from the VPC.

 Correct ;;nswer: D
 C (100%)

 Question #143
 ;; we~ther service provides high-resolution we~ther m~ps from ~ web ~pplic~tion hosted on ;;WS in the eu-west-1  Region. The we~ther m~ps ~re upd~ted frequently ~nd stored in ;;m~zon S3 ~long with st~tic  HTML content. The web ~pplic~tion is fronted by ;;m~zon CloudFront. The comp~ny recently exp~nded to serve users in the us-e~st-1  Region, ~nd these new users report th~t viewing their respective we~ther m~ps is slow from time to time. Which combin~tion of steps will resolve the us-e~st-1 perform~nce issues? (Choose two.)
  ;;. Con gure the ;;WS Glob~l ;;cceler~tor endpoint for the S3 bucket in eu-west-1. Con gure endpoint groups for TCP ports 80 ~nd 443 in us- e~st-1.
  B. Cre~te ~ new S3 bucket in us-e~st-1. Con gure S3 cross-Region replic~tion to synchronize from the S3 bucket in eu-west-1.
  C. Use  L~mbd~@Edge to modify requests from  North ;;meric~ to use the S3 Tr~nsfer ;;cceler~tion endpoint in us-e~st-1.
  D. Use  L~mbd~@Edge to modify requests from  North ;;meric~ to use the S3 bucket in us-e~st-1.
  E. Con gure the ;;WS Glob~l ;;cceler~tor endpoint for us-e~st-1 ~s ~n origin on the CloudFront distribution. Use  L~mbd~@Edge to modify requests from  North ;;meric~ to use the new origin.

 Correct ;;nswer: BD
 BD (95%)                                    3%

 Question #144
 ;; solutions ~rchitect is investig~ting ~n issue in which ~ comp~ny c~nnot est~blish new sessions in ;;m~zon Worksp~ces. ;;n initi~l ~n~lysis indic~tes th~t the issue involves user pro les. The ;;m~zon Worksp~ces environment is con gured to use ;;m~zon  FSx for Windows  File Server ~s the pro le sh~re stor~ge. The  FSx for Windows  File Server  le system is con gured with  10 TB of stor~ge. The solutions ~rchitect discovers th~t the  le system h~s re~ched  Its m~ximum c~p~city. The solutions ~rchitect must ensure th~t users c~n reg~in ~ccess. The solution ~lso must prevent the problem from occurring ~g~in. Which solution will meet these requirements?
  ;;.  Remove old user pro les to cre~te sp~ce.  Migr~te the user pro les to ~n ;;m~zon  FSx for  Lustre  le system.
  B.  Incre~se c~p~city by using the upd~te- le-system comm~nd.  Implement ~n ;;m~zon CloudW~tch metric th~t monitors free sp~ce. Use ;;m~zon  EventBridge to invoke ~n ;;WS  L~mbd~ function to incre~se c~p~city ~s required.
  C.  Monitor the  le system by using the  FreeStor~geC~p~city metric in ;;m~zon CloudW~tch. Use ;;WS Step  Functions to incre~se the c~p~city ~s required.
  D.  Remove old user pro les to cre~te sp~ce. Cre~te ~n ~ddition~l  FSx for Windows  File Server  le system. Upd~te the user pro le redirection for 50% of the users to use the new  le system.

 Correct ;;nswer: C
 B (92%)                                     4%

 Question #145
 ;;n intern~tion~l delivery comp~ny hosts ~ delivery m~n~gement system on ;;WS.  Drivers use the system to uplo~d con rm~tion of delivery. Con rm~tion includes the recipient’s sign~ture or ~ photo of the p~ck~ge with the recipient. The driver’s h~ndheld device uplo~ds sign~tures ~nd photos through  FTP to ~ single ;;m~zon  EC2 inst~nce.  E~ch h~ndheld device s~ves ~  le in ~ directory b~sed on the signed-in user, ~nd the  le n~me m~tches the delivery number. The  EC2 inst~nce then ~dds met~d~t~ to the  le ~fter querying ~ centr~l d~t~b~se to pull delivery inform~tion. The  le is then pl~ced in ;;m~zon S3 for ~rchiving. ;;s the comp~ny exp~nds, drivers report th~t the system is rejecting connections. The  FTP server is h~ving problems bec~use of dropped connections ~nd memory issues in response to these problems, ~ system engineer schedules ~ cron t~sk to reboot the  EC2 inst~nce every 30 minutes. The billing te~m reports th~t  les ~re not ~lw~ys in the ~rchive ~nd th~t the centr~l system is not ~lw~ys upd~ted. ;; solutions ~rchitect needs to design ~ solution th~t m~ximizes sc~l~bility to ensure th~t the ~rchive ~lw~ys receives the  les ~nd th~t systems ~re ~lw~ys upd~ted. The h~ndheld devices c~nnot be modi ed, so the comp~ny c~nnot deploy ~ new ~pplic~tion. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;MI of the existing  EC2 inst~nce. Cre~te ~n ;;uto Sc~ling group of  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Con gure the ;;uto Sc~ling group to h~ve ~ minimum of three inst~nces.
  B. Use ;;WS Tr~nsfer  F~mily to cre~te ~n  FTP server th~t pl~ces the  les in ;;m~zon  El~stic  File System (;;m~zon  EFS).  Mount the  EFS volume to the existing  EC2 inst~nce.  Point the  EC2 inst~nce to the new p~th for  le processing.
  C. Use ;;WS Tr~nsfer  F~mily to cre~te ~n  FTP server th~t pl~ces the  les in ;;m~zon S3. Use ~n S3 event noti c~tion through ;;m~zon Simple Noti c~tion Service (;;m~zon SNS) to invoke ~n ;;WS  L~mbd~ function. Con gure the  L~mbd~ function to ~dd the met~d~t~ ~nd upd~te the delivery system.
  D. Upd~te the h~ndheld devices to pl~ce the  les directly in ;;m~zon S3. Use ~n S3 event noti c~tion through ;;m~zon Simple Queue Service (;;m~zon SQS) to invoke ~n ;;WS  L~mbd~ function. Con gure the  L~mbd~ function to ~dd the met~d~t~ ~nd upd~te the delivery system.

 Correct ;;nswer: B
 C (79%)                                  B (21%)

 Question #146
 ;; comp~ny is running ~n ~pplic~tion in the ;;WS Cloud. The ~pplic~tion runs on cont~iners m ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster. The  ECS t~sks use the  F~rg~te l~unch type. The ~pplic~tion's d~t~ is rel~tion~l ~nd is stored in ;;m~zon ;;uror~  MySQL. To meet regul~tory requirements, the ~pplic~tion must be ~ble to recover to ~ sep~r~te ;;WS  Region in the event of ~n ~pplic~tion f~ilure.  In c~se of ~ f~ilure, no d~t~ c~n be lost. Which solution will meet these requirements with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;.  Provision ~n ;;uror~  Replic~ in ~ different  Region.
  B. Set up ;;WS  D~t~Sync for continuous replic~tion of the d~t~ to ~ different  Region.
  C. Set up ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to perform ~ continuous replic~tion of the d~t~ to ~ different  Region.
  D. Use ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM) to schedule ~ sn~pshot every 5 minutes.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #147
 ;;  n~nci~l services comp~ny receives ~ regul~r d~t~ feed from its credit c~rd servicing p~rtner. ;;pproxim~tely 5,000 records ~re sent every  15 minutes in pl~intext, delivered over  HTTPS directly into ~n ;;m~zon S3 bucket with server-side encryption. This feed cont~ins sensitive credit c~rd prim~ry ~ccount number (P;;N) d~t~. The comp~ny needs to ~utom~tic~lly m~sk the  P;;N before sending the d~t~ to ~nother S3 bucket for ~ddition~l intern~l processing. The comp~ny ~lso needs to remove ~nd merge speci c  elds, ~nd then tr~nsform the record into JSON form~t. ;;ddition~lly, extr~ feeds ~re likely to be ~dded in the future, so ~ny design needs to be e~sily exp~nd~ble. Which solutions will meet these requirements?
  ;;.  Invoke ~n ;;WS  L~mbd~ function on  le delivery th~t extr~cts e~ch record ~nd writes it to ~n ;;m~zon SQS queue.  Invoke ~nother  L~mbd~ function when new mess~ges ~rrive in the SQS queue to process the records, writing the results to ~ tempor~ry loc~tion in ;;m~zon S3.  Invoke ~  n~l  L~mbd~ function once the SQS queue is empty to tr~nsform the records into JSON form~t ~nd send the results to ~nother S3 bucket for intern~l processing.
  B.  Invoke ~n ;;WS  L~mbd~ function on  le delivery th~t extr~cts e~ch record ~nd writes it to ~n ;;m~zon SQS queue. Con gure ~n ;;WS  F~rg~te cont~iner ~pplic~tion to ~utom~tic~lly sc~le to ~ single inst~nce when the SQS queue cont~ins mess~ges.  H~ve the ~pplic~tion process e~ch record, ~nd tr~nsform the record into JSON form~t. When the queue is empty, send the results to ~nother S3 bucket for intern~l processing ~nd sc~le down the ;;WS  F~rg~te inst~nce.
  C. Cre~te ~n ;;WS Glue cr~wler ~nd custom cl~ssi er b~sed on the d~t~ feed form~ts ~nd build ~ t~ble de nition to m~tch.  Invoke ~n ;;WS L~mbd~ function on  le delivery to st~rt ~n ;;WS Glue  ETL job to tr~nsform the entire record ~ccording to the processing ~nd tr~nsform~tion requirements.  De ne the output form~t ~s JSON. Once complete, h~ve the  ETL job send the results to ~nother S3 bucket for intern~l processing.
  D. Cre~te ~n ;;WS Glue cr~wler ~nd custom cl~ssi er b~sed upon the d~t~ feed form~ts ~nd build ~ t~ble de nition to m~tch.  Perform ~n ;;m~zon ;;then~ query on  le delivery to st~rt ~n ;;m~zon  EMR  ETL job to tr~nsform the entire record ~ccording to the processing ~nd tr~nsform~tion requirements.  De ne the output form~t ~s JSON. Once complete, send the results to ~nother S3 bucket for intern~l processing ~nd sc~le down the  EMR cluster.

 Correct ;;nswer: C
 C (100%)

 Question #148
 ;; comp~ny w~nts to use ;;WS to cre~te ~ business continuity solution in c~se the comp~ny's m~in on-premises ~pplic~tion f~ils. The ~pplic~tion runs on physic~l servers th~t ~lso run other ~pplic~tions. The on-premises ~pplic~tion th~t the comp~ny is pl~nning to migr~te uses ~  MySQL d~t~b~se ~s ~ d~t~ store. ;;ll the comp~ny's on-premises ~pplic~tions use oper~ting systems th~t ~re comp~tible with ;;m~zon  EC2. Which solution will ~chieve the comp~ny's go~l with the  LE;;ST oper~tion~l overhe~d?
  ;;.  Inst~ll the ;;WS  Replic~tion ;;gent on the source servers, including the  MySQL servers. Set up replic~tion for ~ll servers.  L~unch test inst~nces for regul~r drills. Cut over to the test inst~nces to f~il over the worklo~d in the c~se of ~ f~ilure event.
  B.  Inst~ll the ;;WS  Replic~tion ;;gent on the source servers, including the  MySQL servers.  Initi~lize ;;WS  El~stic  Dis~ster  Recovery in the t~rget ;;WS  Region.  De ne the l~unch settings.  Frequently perform f~ilover ~nd f~llb~ck from the most recent point in time.
  C. Cre~te ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) replic~tion servers ~nd ~ t~rget ;;m~zon ;;uror~  MySQL  DB cluster to host the d~t~b~se. Cre~te ~  DMS replic~tion t~sk to copy the existing d~t~ to the t~rget  DB cluster. Cre~te ~ loc~l ;;WS Schem~ Conversion Tool (;;WS SCT) ch~nge d~t~ c~pture (CDC) t~sk to keep the d~t~ synchronized.  Inst~ll the rest of the softw~re on  EC2 inst~nces by st~rting with ~ comp~tible b~se ;;MI.
  D.  Deploy ~n ;;WS Stor~ge G~tew~y Volume G~tew~y on premises.  Mount volumes on ~ll on-premises servers.  Inst~ll the ~pplic~tion ~nd the MySQL d~t~b~se on the new volumes. T~ke regul~r sn~pshots.  Inst~ll ~ll the softw~re on  EC2  Inst~nces by st~rting with ~ comp~tible b~se ;;MI.  L~unch ~ Volume G~tew~y on ~n  EC2 inst~nce.  Restore the volumes from the l~test sn~pshot.  Mount the new volumes on the  EC2 inst~nces in the c~se of ~ f~ilure event.

 Correct ;;nswer: C
 B (85%)                                 C (15%)

 Question #149
 ;; comp~ny is subject to regul~tory ~udits of its  n~nci~l inform~tion.  Extern~l ~uditors who use ~ single ;;WS ~ccount need ~ccess to the comp~ny's ;;WS ~ccount. ;; solutions ~rchitect must provide the ~uditors with secure, re~d-only ~ccess to the comp~ny's ;;WS ~ccount. The solution must comply with ;;WS security best pr~ctices. Which solution will meet these requirements?
  ;;.  In the comp~ny's ;;WS ~ccount, cre~te resource policies for ~ll resources in the ~ccount to gr~nt ~ccess to the ~uditors' ;;WS ~ccount. ;;ssign ~ unique extern~l  ID to the resource policy.
  B.  In the comp~ny's ;;WS ~ccount, cre~te ~n  I;;M role th~t trusts the ~uditors' ;;WS ~ccount. Cre~te ~n  I;;M policy th~t h~s the required permissions. ;;tt~ch the policy to the role. ;;ssign ~ unique extern~l  ID to the role's trust policy.
  C.  In the comp~ny's ;;WS ~ccount, cre~te ~n  I;;M user. ;;tt~ch the required  I;;M policies to the  I;;M user. Cre~te ;;PI ~ccess keys for the  I;;M user. Sh~re the ~ccess keys with the ~uditors.
  D.  In the comp~ny's ;;WS ~ccount, cre~te ~n  I;;M group th~t h~s the required permissions. Cre~te ~n  I;;M user in the comp~ny's ~ccount for e~ch ~uditor. ;;dd the  I;;M users to the  I;;M group.

 Correct ;;nswer: B
 B (100%)

 Question #150
 ;; comp~ny h~s ~ l~tency-sensitive tr~ding pl~tform th~t uses ;;m~zon  Dyn~moDB ~s ~ stor~ge b~ckend. The comp~ny con gured the  Dyn~moDB t~ble to use on-dem~nd c~p~city mode. ;; solutions ~rchitect needs to design ~ solution to improve the perform~nce of the tr~ding pl~tform. The new solution must ensure high ~v~il~bility for the tr~ding pl~tform. Which solution will meet these requirements with the  LE;;ST l~tency?
  ;;. Cre~te ~ two-node  Dyn~moDB ;;cceler~tor (D;;X) cluster. Con gure ~n ~pplic~tion to re~d ~nd write d~t~ by using  D;;X.
  B. Cre~te ~ three-node  Dyn~moDB ;;cceler~tor (D;;X) cluster. Con gure ~n ~pplic~tion to re~d d~t~ by using  D;;X ~nd to write d~t~ directly to the  Dyn~moDB t~ble.
  C. Cre~te ~ three-node  Dyn~moDB ;;cceler~tor (D;;X) cluster. Con gure ~n ~pplic~tion to re~d d~t~ directly from the  Dyn~moDB t~ble ~nd to write d~t~ by using  D;;X.
  D. Cre~te ~ single-node  Dyn~moDB ;;cceler~tor (D;;X) cluster. Con gure ~n ~pplic~tion to re~d d~t~ by using  D;;X ~nd to write d~t~ directly to the  Dyn~moDB t~ble.

 Correct ;;nswer: ;;
 B (89%)                                    11%

 Question #151
 ;; comp~ny h~s migr~ted ~n ~pplic~tion from on premises to ;;WS. The ~pplic~tion frontend is ~ st~tic website th~t runs on two ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The ~pplic~tion b~ckend is ~  Python ~pplic~tion th~t runs on three  EC2 inst~nces behind ~nother ;;LB. The  EC2 inst~nces ~re l~rge, gener~l purpose On-Dem~nd  Inst~nces th~t were sized to meet the on-premises speci c~tions for pe~k us~ge of the ~pplic~tion. The ~pplic~tion ~ver~ges hundreds of thous~nds of requests e~ch month.  However, the ~pplic~tion is used m~inly during lunchtime ~nd receives minim~l tr~ c during the rest of the d~y. ;; solutions ~rchitect needs to optimize the infr~structure cost of the ~pplic~tion without neg~tively ~ffecting the ~pplic~tion ~v~il~bility. Which combin~tion of steps will meet these requirements? (Choose two.)
  ;;. Ch~nge ~ll the  EC2 inst~nces to compute optimized inst~nces th~t h~ve the s~me number of cores ~s the existing  EC2 inst~nces.
  B.  Move the ~pplic~tion frontend to ~ st~tic website th~t is hosted on ;;m~zon S3.
  C.  Deploy the ~pplic~tion frontend by using ;;WS  El~stic  Be~nst~lk. Use the s~me inst~nce type for the nodes.
  D. Ch~nge ~ll the b~ckend  EC2 inst~nces to Spot  Inst~nces.
  E.  Deploy the b~ckend  Python ~pplic~tion to gener~l purpose burst~ble  EC2 inst~nces th~t h~ve the s~me number of cores ~s the existing  EC2 inst~nces.

 Correct ;;nswer: BE
 BE (90%)                                   10%

 Question #152
 ;; comp~ny is running ~n event ticketing pl~tform on ;;WS ~nd w~nts to optimize the pl~tform's cost-effectiveness. The pl~tform is deployed on ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) with ;;m~zon  EC2 ~nd is b~cked by ~n ;;m~zon  RDS for  MySQL  DB inst~nce. The comp~ny is developing new ~pplic~tion fe~tures to run on ;;m~zon  EKS with ;;WS  F~rg~te. The pl~tform experiences infrequent high pe~ks in dem~nd. The surges in dem~nd depend on event d~tes. Which solution will provide the  MOST cost-effective setup for the pl~tform?
  ;;.  Purch~se St~nd~rd  Reserved  Inst~nces for the  EC2 inst~nces th~t the  EKS cluster uses in its b~seline lo~d. Sc~le the cluster with Spot Inst~nces to h~ndle pe~ks.  Purch~se  1-ye~r ;;ll Upfront  Reserved  Inst~nces for the d~t~b~se to meet predicted pe~k lo~d for the ye~r.
  B.  Purch~se Compute S~vings  Pl~ns for the predicted medium lo~d of the  EKS cluster. Sc~le the cluster with On-Dem~nd C~p~city Reserv~tions b~sed on event d~tes for pe~ks.  Purch~se  1-ye~r  No Upfront  Reserved  Inst~nces for the d~t~b~se to meet the predicted b~se lo~d. Tempor~rily sc~le out d~t~b~se re~d replic~s during pe~ks.
  C.  Purch~se  EC2  Inst~nce S~vings  Pl~ns for the predicted b~se lo~d of the  EKS cluster. Sc~le the cluster with Spot  Inst~nces to h~ndle pe~ks. Purch~se  1-ye~r ;;ll Upfront  Reserved  Inst~nces for the d~t~b~se to meet the predicted b~se lo~d. Tempor~rily sc~le up the  DB inst~nce m~nu~lly during pe~ks.
  D.  Purch~se Compute S~vings  Pl~ns for the predicted b~se lo~d of the  EKS cluster. Sc~le the cluster with Spot  Inst~nces to h~ndle pe~ks. Purch~se  1-ye~r ;;ll Upfront  Reserved  Inst~nces for the d~t~b~se to meet the predicted b~se lo~d. Tempor~rily sc~le up the  DB inst~nce m~nu~lly during pe~ks.

 Correct ;;nswer: B
 B (80%)                               8%      8%

 Question #153
 ;; comp~ny h~s deployed ~n ~pplic~tion on ;;WS  El~stic  Be~nst~lk. The ~pplic~tion uses ;;m~zon ;;uror~ for the d~t~b~se l~yer. ;;n ;;m~zon CloudFront distribution serves web requests ~nd includes the  El~stic  Be~nst~lk dom~in n~me ~s the origin server. The distribution is con gured with ~n ~ltern~te dom~in n~me th~t visitors use when they ~ccess the ~pplic~tion. E~ch week, the comp~ny t~kes the ~pplic~tion out of service for routine m~inten~nce.  During the time th~t the ~pplic~tion is un~v~il~ble, the comp~ny w~nts visitors to receive ~n inform~tion~l mess~ge inste~d of ~ CloudFront error mess~ge. ;; solutions ~rchitect cre~tes ~n ;;m~zon S3 bucket ~s the  rst step in the process. Which combin~tion of steps should the solutions ~rchitect t~ke next to meet the requirements? (Choose three.)
  ;;. Uplo~d st~tic inform~tion~l content to the S3 bucket.
  B. Cre~te ~ new CloudFront distribution. Set the S3 bucket ~s the origin.
  C. Set the S3 bucket ~s ~ second origin in the origin~l CloudFront distribution. Con gure the distribution ~nd the S3 bucket to use ~n origin ~ccess identity (O;;I).
  D.  During the weekly m~inten~nce, edit the def~ult c~che beh~vior to use the S3 origin.  Revert the ch~nge when the m~inten~nce is complete.
  E.  During the weekly m~inten~nce, cre~te ~ c~che beh~vior for the S3 origin on the new distribution. Set the p~th p~ttern to \ Set the precedence to 0.  Delete the c~che beh~vior when the m~inten~nce is complete.
  F.  During the weekly m~inten~nce, con gure  El~stic  Be~nst~lk to serve tr~ c from the S3 bucket.

 Correct ;;nswer: ;;CD
 ;;CD (100%)

 Question #154
 ;; comp~ny gives users the ~bility to uplo~d im~ges from ~ custom ~pplic~tion. The uplo~d process invokes ~n ;;WS  L~mbd~ function th~t processes ~nd stores the im~ge in ~n ;;m~zon S3 bucket. The ~pplic~tion invokes the  L~mbd~ function by using ~ speci c function version ;;RN. The  L~mbd~ function ~ccepts im~ge processing p~r~meters by using environment v~ri~bles. The comp~ny often ~djusts the environment v~ri~bles of the  L~mbd~ function to ~chieve optim~l im~ge processing output. The comp~ny tests different p~r~meters ~nd publishes ~ new function version with the upd~ted environment v~ri~bles ~fter v~lid~ting results. This upd~te process ~lso requires frequent ch~nges to the custom ~pplic~tion to invoke the new function version ;;RN. These ch~nges c~use interruptions for users. ;; solutions ~rchitect needs to simplify this process to minimize disruption to users. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;.  Directly modify the environment v~ri~bles of the published  L~mbd~ function version. Use the SL;;TEST version to test im~ge processing p~r~meters.
  B. Cre~te ~n ;;m~zon  Dyn~moDB t~ble to store the im~ge processing p~r~meters.  Modify the  L~mbd~ function to retrieve the im~ge processing p~r~meters from the  Dyn~moDB t~ble.
  C.  Directly code the im~ge processing p~r~meters within the  L~mbd~ function ~nd remove the environment v~ri~bles.  Publish ~ new function version when the comp~ny upd~tes the p~r~meters.
  D. Cre~te ~  L~mbd~ function ~li~s.  Modify the client ~pplic~tion to use the function ~li~s ;;RN.  Recon gure the  L~mbd~ ~li~s to point to new versions of the function when the comp~ny  nishes testing.

 Correct ;;nswer: D
 D (100%)

 Question #155
 ;; glob~l medi~ comp~ny is pl~nning ~ multi-Region deployment of ~n ~pplic~tion. ;;m~zon  Dyn~moDB glob~l t~bles will b~ck the deployment to keep the user experience consistent ~cross the two continents where users ~re concentr~ted.  E~ch deployment will h~ve ~ public ;;pplic~tion Lo~d  B~l~ncer (;;LB). The comp~ny m~n~ges public  DNS intern~lly. The comp~ny w~nts to m~ke the ~pplic~tion ~v~il~ble through ~n ~pex dom~in. Which solution will meet these requirements with the  LE;;ST effort?
  ;;.  Migr~te public  DNS to ;;m~zon  Route 53. Cre~te CN;;ME records for the ~pex dom~in to point to the ;;LB. Use ~ geoloc~tion routing policy to route tr~ c b~sed on user loc~tion.
  B.  Pl~ce ~  Network  Lo~d  B~l~ncer (NLB) in front of the ;;LMigr~te public  DNS to ;;m~zon  Route 53. Cre~te ~ CN;;ME record for the ~pex dom~in to point to the  NLB’s st~tic  IP ~ddress. Use ~ geoloc~tion routing policy to route tr~ c b~sed on user loc~tion.
  C. Cre~te ~n ;;WS Glob~l ;;cceler~tor ~cceler~tor with multiple endpoint groups th~t t~rget endpoints in ~ppropri~te ;;WS  Regions. Use the ~cceler~tor’s st~tic  IP ~ddress to cre~te ~ record in public  DNS for the ~pex dom~in.
  D. Cre~te ~n ;;m~zon ;;PI G~tew~y ;;PI th~t is b~cked by ;;WS  L~mbd~ in one of the ;;WS  Regions. Con gure ~  L~mbd~ function to route tr~ c to ~pplic~tion deployments by using the round robin method. Cre~te CN;;ME records for the ~pex dom~in to point to the ;;PI's URL.

 Correct ;;nswer: C
 C (100%)

 Question #156
 ;; comp~ny is developing ~ new serverless ;;PI by using ;;m~zon ;;PI G~tew~y ~nd ;;WS  L~mbd~. The comp~ny integr~ted the  L~mbd~ functions with ;;PI G~tew~y to use sever~l sh~red libr~ries ~nd custom cl~sses. ;; solutions ~rchitect needs to simplify the deployment of the solution ~nd optimize for code reuse. Which solution will meet these requirements?
  ;;.  Deploy the sh~red libr~ries ~nd custom cl~sses into ~  Docker im~ge. Store the im~ge in ~n S3 bucket. Cre~te ~  L~mbd~ l~yer th~t uses the Docker im~ge ~s the source.  Deploy the ;;PI's  L~mbd~ functions ~s Zip p~ck~ges. Con gure the p~ck~ges to use the  L~mbd~ l~yer.
  B.  Deploy the sh~red libr~ries ~nd custom cl~sses to ~  Docker im~ge. Uplo~d the im~ge to ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). Cre~te ~  L~mbd~ l~yer th~t uses the  Docker im~ge ~s the source.  Deploy the ;;PI's  L~mbd~ functions ~s Zip p~ck~ges. Con gure the p~ck~ges to use the  L~mbd~ l~yer.
  C.  Deploy the sh~red libr~ries ~nd custom cl~sses to ~  Docker cont~iner in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) by using the ;;WS F~rg~te l~unch type.  Deploy the ;;PI's  L~mbd~ functions ~s Zip p~ck~ges. Con gure the p~ck~ges to use the deployed cont~iner ~s ~  L~mbd~ l~yer.
  D.  Deploy the sh~red libr~ries, custom cl~sses, ~nd code for the ;;PI's  L~mbd~ functions to ~  Docker im~ge. Uplo~d the im~ge to ;;m~zon El~stic Cont~iner  Registry (;;m~zon  ECR). Con gure the ;;PI's  L~mbd~ functions to use the  Docker im~ge ~s the deployment p~ck~ge.

 Correct ;;nswer: B
 D (67%)                                 B (33%)

 Question #157
 ;; m~nuf~cturing comp~ny is building ~n inspection solution for its f~ctory. The comp~ny h~s  IP c~mer~s ~t the end of e~ch ~ssembly line. The comp~ny h~s used ;;m~zon S~geM~ker to tr~in ~ m~chine le~rning (ML) model to identify common defects from still im~ges. The comp~ny w~nts to provide loc~l feedb~ck to f~ctory workers when ~ defect is detected. The comp~ny must be ~ble to provide this feedb~ck even if the f~ctory’s internet connectivity is down. The comp~ny h~s ~ loc~l  Linux server th~t hosts ~n ;;PI th~t provides loc~l feedb~ck to the workers. How should the comp~ny deploy the  ML model to meet these requirements?
  ;;. Set up ~n ;;m~zon  Kinesis video stre~m from e~ch  IP c~mer~ to ;;WS. Use ;;m~zon  EC2 inst~nces to t~ke still im~ges of the stre~ms. Uplo~d the im~ges to ~n ;;m~zon S3 bucket.  Deploy ~ S~geM~ker endpoint with the  ML model.  Invoke ~n ;;WS  L~mbd~ function to c~ll the inference endpoint when new im~ges ~re uplo~ded. Con gure the  L~mbd~ function to c~ll the loc~l ;;PI when ~ defect is detected.
  B.  Deploy ;;WS  IoT Greengr~ss on the loc~l server.  Deploy the  ML model to the Greengr~ss server. Cre~te ~ Greengr~ss component to t~ke still im~ges from the c~mer~s ~nd run inference. Con gure the component to c~ll the loc~l ;;PI when ~ defect is detected.
  C. Order ~n ;;WS Snowb~ll device.  Deploy ~ S~geM~ker endpoint the  ML model ~nd ~n ;;m~zon  EC2 inst~nce on the Snowb~ll device. T~ke still im~ges from the c~mer~s.  Run inference from the  EC2 inst~nce. Con gure the inst~nce to c~ll the loc~l ;;PI when ~ defect is detected.
  D.  Deploy ;;m~zon  Monitron devices on e~ch  IP c~mer~.  Deploy ~n ;;m~zon  Monitron G~tew~y on premises.  Deploy the  ML model to the ;;m~zon  Monitron devices. Use ;;m~zon  Monitron he~lth st~te ~l~rms to c~ll the loc~l ;;PI from ~n ;;WS  L~mbd~ function when ~ defect is detected.

 Correct ;;nswer: D
 B (92%)                                    8%

 Question #158
 ;; solutions ~rchitect must cre~te ~ business c~se for migr~tion of ~ comp~ny's on-premises d~t~ center to the ;;WS Cloud. The solutions ~rchitect will use ~ con gur~tion m~n~gement d~t~b~se (CMDB) export of ~ll the comp~ny's servers to cre~te the c~se. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Use ;;WS Well-;;rchitected Tool to import the CMDB d~t~ to perform ~n ~n~lysis ~nd gener~te recommend~tions.
  B. Use  Migr~tion  Ev~lu~tor to perform ~n ~n~lysis. Use the d~t~ import templ~te to uplo~d the d~t~ from the CMDB export.
  C.  Implement resource m~tching rules. Use the CMDB export ~nd the ;;WS  Price  List  Bulk ;;PI to query CMDB d~t~ ~g~inst ;;WS services in bulk.
  D. Use ;;WS ;;pplic~tion  Discovery Service to import the CMDB d~t~ to perform ~n ~n~lysis.

 Correct ;;nswer: D
 B (87%)                                   13%

 Question #159
 ;; comp~ny h~s ~ website th~t runs on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The inst~nces ~re in ~n ;;uto Sc~ling group. The ;;LB is ~ssoci~ted with ~n ;;WS W;;F web ;;CL. The website often encounters ~tt~cks in the ~pplic~tion l~yer. The ~tt~cks produce sudden ~nd signi c~nt incre~ses in tr~ c on the ~pplic~tion server. The ~ccess logs show th~t e~ch ~tt~ck origin~tes from different  IP ~ddresses. ;; solutions ~rchitect needs to implement ~ solution to mitig~te these ~tt~cks. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n ;;m~zon CloudW~tch ~l~rm th~t monitors server ~ccess. Set ~ threshold b~sed on ~ccess by  IP ~ddress. Con gure ~n ~l~rm ~ction th~t ~dds the  IP ~ddress to the web ;;CL’s deny list.
  B.  Deploy ;;WS Shield ;;dv~nced in ~ddition to ;;WS W;;F. ;;dd the ;;LB ~s ~ protected resource.
  C. Cre~te ~n ;;m~zon CloudW~tch ~l~rm th~t monitors user  IP ~ddresses. Set ~ threshold b~sed on ~ccess by  IP ~ddress. Con gure the ~l~rm to invoke ~n ;;WS  L~mbd~ function to ~dd ~ deny rule in the ~pplic~tion server’s subnet route t~ble for ~ny  IP ~ddresses th~t ~ctiv~te the ~l~rm.
  D.  Inspect ~ccess logs to  nd ~ p~ttern of  IP ~ddresses th~t l~unched the ~tt~cks. Use ~n ;;m~zon  Route 53 geoloc~tion routing policy to deny tr~ c from the countries th~t host those  IP ~ddresses.

 Correct ;;nswer: C
 B (91%)                                    9%

 Question #160
 ;; comp~ny h~s ~ critic~l ~pplic~tion in which the d~t~ tier is deployed in ~ single ;;WS  Region. The d~t~ tier uses ~n ;;m~zon  Dyn~moDB t~ble ~nd ~n ;;m~zon ;;uror~  MySQL  DB cluster. The current ;;uror~  MySQL engine version supports ~ glob~l d~t~b~se. The ~pplic~tion tier is ~lre~dy deployed in two  Regions. Comp~ny policy st~tes th~t critic~l ~pplic~tions must h~ve ~pplic~tion tier components ~nd d~t~ tier components deployed ~cross two  Regions. The  RTO ~nd  RPO must be no more th~n ~ few minutes e~ch. ;; solutions ~rchitect must recommend ~ solution to m~ke the d~t~ tier compli~nt with comp~ny policy. Which combin~tion of steps will meet these requirements? (Choose two.)
  ;;. ;;dd ~nother  Region to the ;;uror~  MySQL  DB cluster
  B. ;;dd ~nother  Region to e~ch t~ble in the ;;uror~  MySQL  DB cluster
  C. Set up scheduled cross-Region b~ckups for the  Dyn~moDB t~ble ~nd the ;;uror~  MySQL  DB cluster
  D. Convert the existing  Dyn~moDB t~ble to ~ glob~l t~ble by ~dding ~nother  Region to its con gur~tion
  E. Use ;;m~zon  Route 53 ;;pplic~tion  Recovery Controller to ~utom~te d~t~b~se b~ckup ~nd recovery to the second~ry  Region

 Correct ;;nswer: BD
 ;;D (85%)                                 ;;C (15%)

 Question #161
 ;; telecommunic~tions comp~ny is running ~n ~pplic~tion on ;;WS. The comp~ny h~s set up ~n ;;WS  Direct Connect connection between the comp~ny's on-premises d~t~ center ~nd ;;WS. The comp~ny deployed the ~pplic~tion on ;;m~zon  EC2 inst~nces in multiple ;;v~il~bility Zones behind ~n intern~l ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The comp~ny's clients connect from the on-premises network by using  HTTPS. The TLS termin~tes in the ;;LB. The comp~ny h~s multiple t~rget groups ~nd uses p~th-b~sed routing to forw~rd requests b~sed on the URL p~th. The comp~ny is pl~nning to deploy ~n on-premises  rew~ll ~ppli~nce with ~n ~llow list th~t is b~sed on  IP ~ddress. ;; solutions ~rchitect must develop ~ solution to ~llow tr~ c  ow to ;;WS from the on-premises network so th~t the clients c~n continue to ~ccess the ~pplic~tion. Which solution will meet these requirements?
  ;;. Con gure the existing ;;LB to use st~tic  IP ~ddresses. ;;ssign  IP ~ddresses in multiple ;;v~il~bility Zones to the ;;LB. ;;dd the ;;LB  IP ~ddresses to the  rew~ll ~ppli~nce.
  B. Cre~te ~  Network  Lo~d  B~l~ncer (NLB). ;;ssoci~te the  NLB with one st~tic  IP ~ddresses in multiple ;;v~il~bility Zones. Cre~te ~n ;;LB-type t~rget group for the  NLB ~nd ~dd the existing ;;L;;dd the  NLB  IP ~ddresses to the  rew~ll ~ppli~nce. Upd~te the clients to connect to the  NLB.
  C. Cre~te ~  Network  Lo~d  B~l~ncer (NLB). ;;ssoci~te the  LNB with one st~tic  IP ~ddresses in multiple ;;v~il~bility Zones. ;;dd the existing t~rget groups to the  NLB. Upd~te the clients to connect to the  NLB.  Delete the ;;LB ;;dd the  NLB  IP ~ddresses to the  rew~ll ~ppli~nce.
  D. Cre~te ~ G~tew~y  Lo~d  B~l~ncer (GWLB). ;;ssign st~tic  IP ~ddresses to the GWLB in multiple ;;v~il~bility Zones. Cre~te ~n ;;LB-type t~rget group for the GWLB ~nd ~dd the existing ;;LB. ;;dd the GWLB  IP ~ddresses to the  rew~ll ~ppli~nce. Upd~te the clients to connect to the GWLB.

 Correct ;;nswer: ;;
 B (89%)                                   5%

 Question #162
 ;; comp~ny runs ~n ~pplic~tion on ~  eet of ;;m~zon  EC2 inst~nces th~t ~re in priv~te subnets behind ~n internet-f~cing ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The ;;LB is the origin for ~n ;;m~zon CloudFront distribution. ;;n ;;WS W;;F web ;;CL th~t cont~ins v~rious ;;WS m~n~ged rules is ~ssoci~ted with the CloudFront distribution. The comp~ny needs ~ solution th~t will prevent internet tr~ c from directly ~ccessing the ;;LB. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ new web ;;CL th~t cont~ins the s~me rules th~t the existing web ;;CL cont~ins. ;;ssoci~te the new web ;;CL with the ;;LB.
  B. ;;ssoci~te the existing web ;;CL with the ;;LB.
  C. ;;dd ~ security group rule to the ;;LB to ~llow tr~ c from the ;;WS m~n~ged pre x list for CloudFront only.
  D. ;;dd ~ security group rule to the ;;LB to ~llow only the v~rious CloudFront  IP ~ddress r~nges.

 Correct ;;nswer: D
 C (100%)

 Question #163
 ;; comp~ny is running ~n ~pplic~tion th~t uses ~n ;;m~zon  El~stiC~che for  Redis cluster ~s ~ c~ching l~yer. ;; recent security ~udit reve~led th~t the comp~ny h~s con gured encryption ~t rest for  El~stiC~che.  However, the comp~ny did not con gure  El~stiC~che to use encryption in tr~nsit. ;;ddition~lly, users c~n ~ccess the c~che without ~uthentic~tion. ;; solutions ~rchitect must m~ke ch~nges to require user ~uthentic~tion ~nd to ensure th~t the comp~ny is using end-to-end encryption. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;UTH token. Store the token in ;;WS System  M~n~ger  P~r~meter Store, ~s ~n encrypted p~r~meter. Cre~te ~ new cluster with ;;UTH, ~nd con gure encryption in tr~nsit. Upd~te the ~pplic~tion to retrieve the ;;UTH token from  P~r~meter Store when necess~ry ~nd to use the ;;UTH token for ~uthentic~tion.
  B. Cre~te ~n ;;UTH token. Store the token in ;;WS Secrets  M~n~ger. Con gure the existing cluster to use the ;;UTH token, ~nd con gure encryption in tr~nsit. Upd~te the ~pplic~tion to retrieve the ;;UTH token from Secrets  M~n~ger when necess~ry ~nd to use the ;;UTH token for ~uthentic~tion.
  C. Cre~te ~n SSL certi c~te. Store the certi c~te in ;;WS Secrets  M~n~ger. Cre~te ~ new cluster, ~nd con gure encryption in tr~nsit. Upd~te the ~pplic~tion to retrieve the SSL certi c~te from Secrets  M~n~ger when necess~ry ~nd to use the certi c~te for ~uthentic~tion.
  D. Cre~te ~n SSL certi c~te. Store the certi c~te in ;;WS Systems  M~n~ger  P~r~meter Store, ~s ~n encrypted ~dv~nced p~r~meter. Upd~te the existing cluster to con gure encryption in tr~nsit. Upd~te the ~pplic~tion to retrieve the SSL certi c~te from  P~r~meter Store when necess~ry ~nd to use the certi c~te for ~uthentic~tion.

 Correct ;;nswer: C
 B (100%)

 Question #164
 ;; comp~ny is running ~ compute worklo~d by using ;;m~zon  EC2 Spot  Inst~nces th~t ~re in ~n ;;uto Sc~ling group. The l~unch templ~te uses two pl~cement groups ~nd ~ single inst~nce type. Recently, ~ monitoring system reported ;;uto Sc~ling inst~nce l~unch f~ilures th~t correl~ted with longer w~it times for system users. The comp~ny needs to improve the over~ll reli~bility of the worklo~d. Which solution will meet this requirement?
  ;;.  Repl~ce the l~unch templ~te with ~ l~unch con gur~tion to use ~n ;;uto Sc~ling group th~t uses ~ttribute-b~sed inst~nce type selection.
  B. Cre~te ~ new l~unch templ~te version th~t uses ~ttribute-b~sed inst~nce type selection. Con gure the ;;uto Sc~ling group to use the new l~unch templ~te version.
  C. Upd~te the l~unch templ~te ;;uto Sc~ling group to incre~se the number of pl~cement groups.
  D. Upd~te the l~unch templ~te to use ~ l~rger inst~nce type.

 Correct ;;nswer: C
 B (100%)

 Question #165
 ;; comp~ny is migr~ting ~ document processing worklo~d to ;;WS. The comp~ny h~s upd~ted m~ny ~pplic~tions to n~tively use the ;;m~zon S3 ;;PI to store, retrieve, ~nd modify documents th~t ~ processing server gener~tes ~t ~ r~te of ~pproxim~tely 5 documents every second. ;;fter the document processing is  nished, customers c~n downlo~d the documents directly from ;;m~zon S3. During the migr~tion, the comp~ny discovered th~t it could not immedi~tely upd~te the processing server th~t gener~tes m~ny documents to support the S3 ;;PI. The server runs on  Linux ~nd requires f~st loc~l ~ccess to the  les th~t the server gener~tes ~nd modi es. When the server  nishes processing, the  les must be ~v~il~ble to the public for downlo~d within 30 minutes. Which solution will meet these requirements with the  LE;;ST ~mount of effort?
  ;;.  Migr~te the ~pplic~tion to ~n ;;WS  L~mbd~ function. Use the ;;WS SDK for J~v~ to gener~te, modify, ~nd ~ccess the  les th~t the comp~ny stores directly in ;;m~zon S3.
  B. Set up ~n ;;m~zon S3  File G~tew~y ~nd con gure ~  le sh~re th~t is linked to the document store.  Mount the  le sh~re on ~n ;;m~zon  EC2 inst~nce by using  NFS. When ch~nges occur in ;;m~zon S3, initi~te ~  RefreshC~che ;;PI c~ll to upd~te the S3  File G~tew~y.
  C. Con gure ;;m~zon  FSx for  Lustre with ~n import ~nd export policy.  Link the new  le system to ~n S3 bucket.  Inst~ll the  Lustre client ~nd mount the document store to ~n ;;m~zon  EC2 inst~nce by using  NFS.
  D. Con gure ;;WS  D~t~Sync to connect to ~n ;;m~zon  EC2 inst~nce. Con gure ~ t~sk to synchronize the gener~ted  les to ~nd from ;;m~zon S3.

 Correct ;;nswer: C
 B (60%)                                C (35%)           5%

 Question #166
 ;; delivery comp~ny is running ~ serverless solution in the ;;WS Cloud. The solution m~n~ges user d~t~, delivery inform~tion, ~nd p~st purch~se det~ils. The solution consists of sever~l microservices. The centr~l user service stores sensitive d~t~ in ~n ;;m~zon  Dyn~moDB t~ble. Sever~l of the other microservices store ~ copy of p~rts of the sensitive d~t~ in different stor~ge services. The comp~ny needs the ~bility to delete user inform~tion upon request. ;;s soon ~s the centr~l user service deletes ~ user, every other microservice must ~lso delete its copy of the d~t~ immedi~tely. Which solution will meet these requirements?
  ;;. ;;ctiv~te  Dyn~moDB Stre~ms on the  Dyn~moDB t~ble. Cre~te ~n ;;WS  L~mbd~ trigger for the  Dyn~moDB stre~m th~t will post events ~bout user deletion in ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Con gure e~ch microservice to poll the queue ~nd delete the user from the  Dyn~moDB t~ble.
  B. Set up  Dyn~moDB event noti c~tions on the  Dyn~moDB t~ble. Cre~te ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic ~s ~ t~rget for the  Dyn~moDB event noti c~tion. Con gure e~ch microservice to subscribe to the SNS topic ~nd to delete the user from the Dyn~moDB t~ble.
  C. Con gure the centr~l user service to post ~n event on ~ custom ;;m~zon  EventBridge event bus when the comp~ny deletes ~ user. Cre~te ~n EventBridge rule for e~ch microservice to m~tch the user deletion event p~ttern ~nd invoke logic in the microservice to delete the user from the  Dyn~moDB t~ble.
  D. Con gure the centr~l user service to post ~ mess~ge on ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue when the comp~ny deletes ~ user. Con gure e~ch microservice to cre~te ~n event  lter on the SQS queue ~nd to delete the user from the  Dyn~moDB t~ble.

 Correct ;;nswer: D
 C (71%)                               ;; (24%)       6%

 Question #167
 ;; comp~ny is running ~ web ~pplic~tion in ~ VPC. The web ~pplic~tion runs on ~ group of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d B~l~ncer (;;LB). The ;;LB is using ;;WS W;;F. ;;n extern~l customer needs to connect to the web ~pplic~tion. The comp~ny must provide  IP ~ddresses to ~ll extern~l customers. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;.  Repl~ce the ;;LB with ~  Network  Lo~d  B~l~ncer (NLB). ;;ssign ~n  El~stic  IP ~ddress to the  NLB.
  B. ;;lloc~te ~n  El~stic  IP ~ddress. ;;ssign the  El~stic  IP ~ddress to the ;;LProvide the  El~stic  IP ~ddress to the customer.
  C. Cre~te ~n ;;WS Glob~l ;;cceler~tor st~nd~rd ~cceler~tor. Specify the ;;LB ~s the ~cceler~tor's endpoint.  Provide the ~cceler~tor's  IP ~ddresses to the customer.
  D. Con gure ~n ;;m~zon CloudFront distribution. Set the ;;LB ~s the origin.  Ping the distribution's  DNS n~me to determine the distribution's public  IP ~ddress.  Provide the  IP ~ddress to the customer.

 Correct ;;nswer: B
 C (90%)                                    7%

 Question #168
 ;; comp~ny h~s ~ few ;;WS ~ccounts for development ~nd w~nts to move its production ~pplic~tion to ;;WS. The comp~ny needs to enforce ;;m~zon  El~stic  Block Store (;;m~zon  EBS) encryption ~t rest current production ~ccounts ~nd future production ~ccounts only. The comp~ny needs ~ solution th~t includes built-in blueprints ~nd gu~rdr~ils. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Use ;;WS CloudForm~tion St~ckSets to deploy ;;WS Con g rules on production ~ccounts.
  B. Cre~te ~ new ;;WS Control Tower l~nding zone in ~n existing developer ~ccount. Cre~te OUs for ~ccounts. ;;dd production ~nd development ~ccounts to production ~nd development OUs, respectively.
  C. Cre~te ~ new ;;WS Control Tower l~nding zone in the comp~ny’s m~n~gement ~ccount. ;;dd production ~nd development ~ccounts to production ~nd development OUs. respectively.
  D.  Invite existing ~ccounts to join the org~niz~tion in ;;WS Org~niz~tions. Cre~te SCPs to ensure compli~nce.
  E. Cre~te ~ gu~rdr~il from the m~n~gement ~ccount to detect  EBS encryption.
  F. Cre~te ~ gu~rdr~il for the production OU to detect  EBS encryption.

 Correct ;;nswer: BCE
 CDF (74%)                            11%       Other

 Question #169
 ;; comp~ny is running ~ critic~l st~teful web ~pplic~tion on two  Linux ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) with ~n ;;m~zon  RDS for  MySQL d~t~b~se. The comp~ny hosts the  DNS records for the ~pplic~tion in ;;m~zon  Route 53. ;; solutions ~rchitect must recommend ~ solution to improve the resiliency of the ~pplic~tion. The solution must meet the following objectives: • ;;pplic~tion tier:  RPO of 2 minutes.  RTO of 30 minutes •  D~t~b~se tier:  RPO of 5 minutes.  RTO of 30 minutes The comp~ny does not w~nt to m~ke signi c~nt ch~nges to the existing ~pplic~tion ~rchitecture. The comp~ny must ensure optim~l l~tency ~fter ~ f~ilover. Which solution will meet these requirements?
  ;;. Con gure the  EC2 inst~nces to use ;;WS  El~stic  Dis~ster  Recovery. Cre~te ~ cross-Region re~d replic~ for the  RDS  DB inst~nce. Cre~te ~n ;;LB in ~ second ;;WS  Region. Cre~te ~n ;;WS Glob~l ;;cceler~tor endpoint, ~nd ~ssoci~te the endpoint with the ;;LBs. Upd~te  DNS records to point to the Glob~l ;;cceler~tor endpoint.
  B. Con gure the  EC2 inst~nces to use ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM) to t~ke sn~pshots of the  EBS volumes. Con gure  RDS ~utom~ted b~ckups. Con gure b~ckup replic~tion to ~ second ;;WS  Region. Cre~te ~n ;;LB in the second  Region. Cre~te ~n ;;WS Glob~l ;;cceler~tor endpoint, ~nd ~ssoci~te the endpoint with the ;;LBs. Upd~te  DNS records to point to the Glob~l ;;cceler~tor endpoint.
  C. Cre~te ~ b~ckup pl~n in ;;WS  B~ckup for the  EC2 inst~nces ~nd  RDS  DB inst~nce. Con gure b~ckup replic~tion to ~ second ;;WS  Region. Cre~te ~n ;;LB in the second  Region. Con gure ~n ;;m~zon CloudFront distribution in front of the ;;LB. Upd~te  DNS records to point to CloudFront.
  D. Con gure the  EC2 inst~nces to use ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM) to t~ke sn~pshots of the  EBS volumes. Cre~te ~ cross- Region re~d replic~ for the  RDS  DB inst~nce. Cre~te ~n ;;LB in ~ second ;;WS  Region. Cre~te ~n ;;WS Glob~l ;;cceler~tor endpoint, ~nd ~ssoci~te the endpoint with the ;;LBs.

 Correct ;;nswer: B
 ;; (95%)                                    5%

 Question #170
 ;; solutions ~rchitect w~nts to cost-optimize ~nd ~ppropri~tely size ;;m~zon  EC2 inst~nces in ~ single ;;WS ~ccount. The solutions ~rchitect w~nts to ensure th~t the inst~nces ~re optimized b~sed on CPU, memory, ~nd network metrics. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;.  Purch~se ;;WS  Business Support or ;;WS  Enterprise Support for the ~ccount.
  B. Turn on ;;WS Trusted ;;dvisor ~nd review ~ny “Low Utiliz~tion ;;m~zon  EC2  Inst~nces” recommend~tions.
  C.  Inst~ll the ;;m~zon CloudW~tch ~gent ~nd con gure memory metric collection on the  EC2 inst~nces.
  D. Con gure ;;WS Compute Optimizer in the ;;WS ~ccount to receive  ndings ~nd optimiz~tion recommend~tions.
  E. Cre~te ~n  EC2  Inst~nce S~vings  Pl~n for the ;;WS  Regions, inst~nce f~milies, ~nd oper~ting systems of interest.

 Correct ;;nswer: BD
 CD (90%)                                   10%

 Question #171
 ;; comp~ny uses ~n ;;WS CodeCommit repository. The comp~ny must store ~ b~ckup copy of the d~t~ th~t is in the repository in ~ second ;;WS Region. Which solution will meet these requirements?
  ;;. Con gure ;;WS  El~stic  Dis~ster  Recovery to replic~te the CodeCommit repository d~t~ to the second  Region.
  B. Use ;;WS  B~ckup to b~ck up the CodeCommit repository on ~n hourly schedule. Cre~te ~ cross-Region copy in the second  Region.
  C. Cre~te ~n ;;m~zon  EventBridge rule to invoke ;;WS CodeBuild when the comp~ny pushes code to the repository. Use CodeBuild to clone the repository. Cre~te ~ .zip  le of the content. Copy the  le to ~n S3 bucket in the second  Region.
  D. Cre~te ~n ;;WS Step  Functions work ow on ~n hourly schedule to t~ke ~ sn~pshot of the CodeCommit repository. Con gure the work ow to copy the sn~pshot to ~n S3 bucket in the second  Region

 Correct ;;nswer: C
 C (95%)                                    5%

 Question #172
 ;; comp~ny h~s multiple business units th~t e~ch h~ve sep~r~te ~ccounts on ;;WS.  E~ch business unit m~n~ges its own network with sever~l VPCs th~t h~ve CIDR r~nges th~t overl~p. The comp~ny’s m~rketing te~m h~s cre~ted ~ new intern~l ~pplic~tion ~nd w~nts to m~ke the ~pplic~tion ~ccessible to ~ll the other business units. The solution must use priv~te  IP ~ddresses only. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;.  Instruct e~ch business unit to ~dd ~ unique second~ry CIDR r~nge to the business unit's VPC.  Peer the VPCs ~nd use ~ priv~te  N;;T g~tew~y in the second~ry r~nge to route tr~ c to the m~rketing te~m.
  B. Cre~te ~n ;;m~zon  EC2 inst~nce to serve ~s ~ virtu~l ~ppli~nce in the m~rketing ~ccount's VPC. Cre~te ~n ;;WS Site-to-Site VPN connection between the m~rketing te~m ~nd e~ch business unit's VPC.  Perform  N;;T where necess~ry.
  C. Cre~te ~n ;;WS  Priv~teLink endpoint service to sh~re the m~rketing ~pplic~tion. Gr~nt permission to speci c ;;WS ~ccounts to connect to the service. Cre~te interf~ce VPC endpoints in other ~ccounts to ~ccess the ~pplic~tion by using priv~te  IP ~ddresses.
  D. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) in front of the m~rketing ~pplic~tion in ~ priv~te subnet. Cre~te ~n ;;PI G~tew~y ;;PI. Use the ;;m~zon ;;PI G~tew~y priv~te integr~tion to connect the ;;PI to the  NLB. ;;ctiv~te  I;;M ~uthoriz~tion for the ;;PI. Gr~nt ~ccess to the ~ccounts of the other business units.

 Correct ;;nswer: D
 C (93%)                                    7%

 Question #173
 ;; comp~ny needs to ~udit the security posture of ~ newly ~cquired ;;WS ~ccount. The comp~ny’s d~t~ security te~m requires ~ noti c~tion only when ~n ;;m~zon S3 bucket becomes publicly exposed. The comp~ny h~s ~lre~dy est~blished ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic th~t h~s the d~t~ security te~m's em~il ~ddress subscribed. Which solution will meet these requirements?
  ;;. Cre~te ~n S3 event noti c~tion on ~ll S3 buckets for the isPublic event. Select the SNS topic ~s the t~rget for the event noti c~tions.
  B. Cre~te ~n ~n~lyzer in ;;WS  Identity ~nd ;;ccess  M~n~gement ;;ccess ;;n~lyzer. Cre~te ~n ;;m~zon  EventBridge rule for the event type “;;ccess ;;n~lyzer  Finding” with ~  lter for “isPublic: true.” Select the SNS topic ~s the  EventBridge rule t~rget.
  C. Cre~te ~n ;;m~zon  EventBridge rule for the event type “Bucket-Level ;;PI C~ll vi~ CloudTr~il” with ~  lter for “PutBucketPolicy.” Select the SNS topic ~s the  EventBridge rule t~rget.
  D. ;;ctiv~te ;;WS Con g ~nd ~dd the cloudtr~il-s3-d~t~events-en~bled rule. Cre~te ~n ;;m~zon  EventBridge rule for the event type “Con g  Rules Re-ev~lu~tion St~tus” with ~  lter for “NON_COMPLI;;NT.” Select the SNS topic ~s the  EventBridge rule t~rget.

 Correct ;;nswer: ;;
 B (94%)                                       6%

 Question #174
 ;; solutions ~rchitect needs to ~ssess ~ newly ~cquired comp~ny’s portfolio of ~pplic~tions ~nd d~t~b~ses. The solutions ~rchitect must cre~te ~ business c~se to migr~te the portfolio to ;;WS. The newly ~cquired comp~ny runs ~pplic~tions in ~n on-premises d~t~ center. The d~t~ center is not well documented. The solutions ~rchitect c~nnot immedi~tely determine how m~ny ~pplic~tions ~nd d~t~b~ses exist. Tr~ c for the ~pplic~tions is v~ri~ble. Some ~pplic~tions ~re b~tch processes th~t run ~t the end of e~ch month. The solutions ~rchitect must g~in ~ better underst~nding of the portfolio before ~ migr~tion to ;;WS c~n begin. Which solution will meet these requirements?
  ;;. Use ;;WS Server  Migr~tion Service (;;WS SMS) ~nd ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to ev~lu~te migr~tion. Use ;;WS Service C~t~log to underst~nd ~pplic~tion ~nd d~t~b~se dependencies.
  B. Use ;;WS ;;pplic~tion  Migr~tion Service.  Run ~gents on the on-premises infr~structure.  M~n~ge the ~gents by using ;;WS  Migr~tion  Hub. Use ;;WS Stor~ge G~tew~y to ~ssess loc~l stor~ge needs ~nd d~t~b~se dependencies.
  C. Use  Migr~tion  Ev~lu~tor to gener~te ~ list of servers.  Build ~ report for ~ business c~se. Use ;;WS  Migr~tion  Hub to view the portfolio. Use ;;WS ;;pplic~tion  Discovery Service to g~in ~n underst~nding of ~pplic~tion dependencies.
  D. Use ;;WS Control Tower in the destin~tion ~ccount to gener~te ~n ~pplic~tion portfolio. Use ;;WS Server  Migr~tion Service (;;WS SMS) to gener~te deeper reports ~nd ~ business c~se. Use ~ l~nding zone for core ~ccounts ~nd resources.

 Correct ;;nswer: B
 C (96%)                                    4%

 Question #175
 ;; comp~ny h~s ~n ~pplic~tion th~t runs ~s ~  Replic~Set of multiple pods in ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster. The  EKS cluster h~s nodes in multiple ;;v~il~bility Zones. The ~pplic~tion gener~tes m~ny sm~ll  les th~t must be ~ccessible ~cross ~ll running inst~nces of the ~pplic~tion. The comp~ny needs to b~ck up the  les ~nd ret~in the b~ckups for  1 ye~r. Which solution will meet these requirements while providing the  F;;STEST stor~ge perform~nce?
  ;;. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system ~nd ~ mount t~rget for e~ch subnet th~t cont~ins nodes in the  EKS cluster. Con gure the  Replic~Set to mount the  le system.  Direct the ~pplic~tion to store  les in the  le system. Con gure ;;WS  B~ckup to b~ck up ~nd ret~in copies of the d~t~ for  1 ye~r.
  B. Cre~te ~n ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume.  En~ble the  EBS  Multi-;;tt~ch fe~ture. Con gure the  Replic~Set to mount the EBS volume.  Direct the ~pplic~tion to store  les in the  EBS volume. Con gure ;;WS  B~ckup to b~ck up ~nd ret~in copies of the d~t~ for  1 ye~r.
  C. Cre~te ~n ;;m~zon S3 bucket. Con gure the  Replic~Set to mount the S3 bucket.  Direct the ~pplic~tion to store  les in the S3 bucket. Con gure S3 Versioning to ret~in copies of the d~t~. Con gure ~n S3  Lifecycle policy to delete objects ~fter  1 ye~r.
  D. Con gure the  Replic~Set to use the stor~ge ~v~il~ble on e~ch of the running ~pplic~tion pods to store the  les loc~lly. Use ~ third-p~rty tool to b~ck up the  EKS cluster for  1 ye~r.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #176
 ;; comp~ny runs ~ customer service center th~t ~ccepts c~lls ~nd ~utom~tic~lly sends ~ll customers ~ m~n~ged, inter~ctive, two-w~y experience survey by text mess~ge. The ~pplic~tions th~t support the customer service center run on m~chines th~t the comp~ny hosts in ~n on-premises d~t~ center. The h~rdw~re th~t the comp~ny uses is old, ~nd the comp~ny is experiencing downtime with the system. The comp~ny w~nts to migr~te the system to ;;WS to improve reli~bility. Which solution will meet these requirements with the  LE;;ST ongoing oper~tion~l overhe~d?
  ;;. Use ;;m~zon Connect to repl~ce the old c~ll center h~rdw~re. Use ;;m~zon  Pinpoint to send text mess~ge surveys to customers.
  B. Use ;;m~zon Connect to repl~ce the old c~ll center h~rdw~re. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to send text mess~ge surveys to customers.
  C.  Migr~te the c~ll center softw~re to ;;m~zon  EC2 inst~nces th~t ~re in ~n ;;uto Sc~ling group. Use the  EC2 inst~nces to send text mess~ge surveys to customers.
  D. Use ;;m~zon  Pinpoint to repl~ce the old c~ll center h~rdw~re ~nd to send text mess~ge surveys to customers.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #177
 ;; comp~ny is building ~ c~ll center by using ;;m~zon Connect. The comp~ny’s oper~tions te~m is de ning ~ dis~ster recovery (DR) str~tegy ~cross ;;WS  Regions. The cont~ct center h~s dozens of cont~ct  ows, hundreds of users, ~nd dozens of cl~imed phone numbers. Which solution will provide  DR with the  LOWEST  RTO?
  ;;. Cre~te ~n ;;WS  L~mbd~ function to check the ~v~il~bility of the ;;m~zon Connect inst~nce ~nd to send ~ noti c~tion to the oper~tions te~m in c~se of un~v~il~bility. Cre~te ~n ;;m~zon  EventBridge rule to invoke the  L~mbd~ function every 5 minutes. ;;fter noti c~tion, instruct the oper~tions te~m to use the ;;WS  M~n~gement Console to provision ~ new ;;m~zon Connect inst~nce in ~ second  Region.  Deploy the cont~ct  ows, users, ~nd cl~imed phone numbers by using ~n ;;WS CloudForm~tion templ~te.
  B.  Provision ~ new ;;m~zon Connect inst~nce with ~ll existing users in ~ second  Region. Cre~te ~n ;;WS  L~mbd~ function to check the ~v~il~bility of the ;;m~zon Connect inst~nce. Cre~te ~n ;;m~zon  EventBridge rule to invoke the  L~mbd~ function every 5 minutes.  In the event of ~n issue, con gure the  L~mbd~ function to deploy ~n ;;WS CloudForm~tion templ~te th~t provisions cont~ct  ows ~nd cl~imed numbers in the second  Region.
  C.  Provision ~ new ;;m~zon Connect inst~nce with ~ll existing cont~ct  ows ~nd cl~imed phone numbers in ~ second  Region. Cre~te ~n ;;m~zon  Route 53 he~lth check for the URL of the ;;m~zon Connect inst~nce. Cre~te ~n ;;m~zon CloudW~tch ~l~rm for f~iled he~lth checks. Cre~te ~n ;;WS  L~mbd~ function to deploy ~n ;;WS CloudForm~tion templ~te th~t provisions ~ll users. Con gure the ~l~rm to invoke the L~mbd~ function.
  D.  Provision ~ new ;;m~zon Connect inst~nce with ~ll existing users ~nd cont~ct  ows in ~ second  Region. Cre~te ~n ;;m~zon  Route 53 he~lth check for the URL of the ;;m~zon Connect inst~nce. Cre~te ~n ;;m~zon CloudW~tch ~l~rm for f~iled he~lth checks. Cre~te ~n ;;WS  L~mbd~ function to deploy ~n ;;WS CloudForm~tion templ~te th~t provisions cl~imed phone numbers. Con gure the ~l~rm to invoke the  L~mbd~ function.

 Correct ;;nswer: D
 D (84%)                                 B (16%)

 Question #178
 ;; comp~ny runs ~n ~pplic~tion on ;;WS. The comp~ny cur~tes d~t~ from sever~l different sources. The comp~ny uses propriet~ry ~lgorithms to perform d~t~ tr~nsform~tions ~nd ~ggreg~tions. ;;fter the comp~ny performs  ETL processes, the comp~ny stores the results in ;;m~zon  Redshift t~bles. The comp~ny sells this d~t~ to other comp~nies. The comp~ny downlo~ds the d~t~ ~s  les from the ;;m~zon  Redshift t~bles ~nd tr~nsmits the  les to sever~l d~t~ customers by using  FTP. The number of d~t~ customers h~s grown signi c~ntly.  M~n~gement of the d~t~ customers h~s become di cult. The comp~ny will use ;;WS  D~t~  Exch~nge to cre~te ~ d~t~ product th~t the comp~ny c~n use to sh~re d~t~ with customers. The comp~ny w~nts to con rm the identities of the customers before the comp~ny sh~res d~t~. The customers ~lso need ~ccess to the most recent d~t~ when the comp~ny publishes the d~t~. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Use ;;WS  D~t~  Exch~nge for ;;PIs to sh~re d~t~ with customers. Con gure subscription veri c~tion.  In the ;;WS ~ccount of the comp~ny th~t produces the d~t~, cre~te ~n ;;m~zon ;;PI G~tew~y  D~t~ ;;PI service integr~tion with ;;m~zon  Redshift.  Require the d~t~ customers to subscribe to the d~t~ product.
  B.  In the ;;WS ~ccount of the comp~ny th~t produces the d~t~, cre~te ~n ;;WS  D~t~  Exch~nge d~t~sh~re by connecting ;;WS  D~t~  Exch~nge to the  Redshift cluster. Con gure subscription veri c~tion.  Require the d~t~ customers to subscribe to the d~t~ product.
  C.  Downlo~d the d~t~ from the ;;m~zon  Redshift t~bles to ~n ;;m~zon S3 bucket periodic~lly. Use ;;WS  D~t~  Exch~nge for S3 to sh~re d~t~ with customers. Con gure subscription veri c~tion.  Require the d~t~ customers to subscribe to the d~t~ product.
  D.  Publish the ;;m~zon  Redshift d~t~ to ~n Open  D~t~ on ;;WS  D~t~  Exch~nge.  Require the customers to subscribe to the d~t~ product in ;;WS D~t~  Exch~nge.  In the ;;WS ~ccount of the comp~ny th~t produces the d~t~, ~tt~ch  I;;M resource-b~sed policies to the ;;m~zon  Redshift t~bles to ~llow ~ccess only to veri ed ;;WS ~ccounts.

 Correct ;;nswer: B
 B (86%)                                   14%

 Question #179
 ;; solutions ~rchitect is designing ~ solution to process events. The solution must h~ve the ~bility to sc~le in ~nd out b~sed on the number of events th~t the solution receives.  If ~ processing error occurs, the event must move into ~ sep~r~te queue for review. Which solution will meet these requirements?
  ;;. Send event det~ils to ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic. Con gure ~n ;;WS  L~mbd~ function ~s ~ subscriber to the SNS topic to process the events. ;;dd ~n on-f~ilure destin~tion to the function. Set ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue ~s the t~rget.
  B.  Publish events to ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Cre~te ~n ;;m~zon  EC2 ;;uto Sc~ling group. Con gure the ;;uto Sc~ling group to sc~le in ~nd out b~sed on the ;;pproxim~te;;geOfOldestMess~ge metric of the queue. Con gure the ~pplic~tion to write f~iled mess~ges to ~ de~d-letter queue.
  C. Write events to ~n ;;m~zon  Dyn~moDB t~ble. Con gure ~  Dyn~moDB stre~m for the t~ble. Con gure the stre~m to invoke ~n ;;WS  L~mbd~ function. Con gure the  L~mbd~ function to process the events.
  D.  Publish events to ~n ;;m~zon  EventBndge event bus. Cre~te ~nd run ~n ~pplic~tion on ~n ;;m~zon  EC2 inst~nce with ~n ;;uto Sc~ling group th~t is behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Set the ;;LB ~s the event bus t~rget. Con gure the event bus to retry events. Write mess~ges to ~ de~d-letter queue if the ~pplic~tion c~nnot process the mess~ges.

 Correct ;;nswer: B
 B (50%)                                  ;; (50%)

 Question #180
 ;; comp~ny runs ~ processing engine in the ;;WS Cloud. The engine processes environment~l d~t~ from logistics centers to c~lcul~te ~ sust~in~bility index. The comp~ny h~s millions of devices in logistics centers th~t ~re spre~d ~cross  Europe. The devices send inform~tion to the processing engine through ~  RESTful ;;PI. The ;;PI experiences unpredict~ble bursts of tr~ c. The comp~ny must implement ~ solution to process ~ll d~t~ th~t the devices send to the processing engine.  D~t~ loss is un~ccept~ble. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) for the  RESTful ;;PI. Cre~te ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Cre~te ~ listener ~nd ~ t~rget group for the ;;LB ;;dd the SQS queue ~s the t~rget. Use ~ cont~iner th~t runs in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the  F~rg~te l~unch type to process mess~ges in the queue.
  B. Cre~te ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI th~t implements the  RESTful ;;PI. Cre~te ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Cre~te ~n ;;PI G~tew~y service integr~tion with the SQS queue. Cre~te ~n ;;WS  L~mbd~ function to process mess~ges in the SQS queue.
  C. Cre~te ~n ;;m~zon ;;PI G~tew~y  REST ;;PI th~t implements the  RESTful ;;PI. Cre~te ~  eet of ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group. Cre~te ~n ;;PI G~tew~y ;;uto Sc~ling group proxy integr~tion. Use the  EC2 inst~nces to process incoming d~t~.
  D. Cre~te ~n ;;m~zon CloudFront distribution for the  RESTful ;;PI. Cre~te ~ d~t~ stre~m in ;;m~zon  Kinesis  D~t~ Stre~ms. Set the d~t~ stre~m ~s the origin for the distribution. Cre~te ~n ;;WS  L~mbd~ function to consume ~nd process d~t~ in the d~t~ stre~m.

 Correct ;;nswer: B
 B (88%)                                     9%

 Question #181
 ;; comp~ny is designing its network con gur~tion in the ;;WS Cloud. The comp~ny uses ;;WS Org~niz~tions to m~n~ge ~ multi-~ccount setup. The comp~ny h~s three OUs.  E~ch OU cont~ins more th~n  100 ;;WS ~ccounts.  E~ch ~ccount h~s ~ single VPC, ~nd ~ll the VPCs in e~ch OU ~re in the s~me ;;WS  Region. The CIDR r~nges for ~ll the ;;WS ~ccounts do not overl~p. The comp~ny needs to implement ~ solution in which VPCs in the s~me OU c~n communic~te with e~ch other but c~nnot communic~te with VPCs in other OUs. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n ;;WS CloudForm~tion st~ck set th~t est~blishes VPC peering between ~ccounts in e~ch OU.  Provision the st~ck set in e~ch OU.
  B.  In e~ch OU, cre~te ~ dedic~ted networking ~ccount th~t h~s ~ single VPC. Sh~re this VPC with ~ll the other ~ccounts in the OU by using ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M). Cre~te ~ VPC peering connection between the networking ~ccount ~nd e~ch ~ccount in the OU.
  C.  Provision ~ tr~nsit g~tew~y in ~n ~ccount in e~ch OU. Sh~re the tr~nsit g~tew~y ~cross the org~niz~tion by using ;;WS  Resource ;;ccess M~n~ger (;;WS  R;;M). Cre~te tr~nsit g~tew~y VPC ~tt~chments for e~ch VPC.
  D.  In e~ch OU, cre~te ~ dedic~ted networking ~ccount th~t h~s ~ single VPC.  Est~blish ~ VPN connection between the networking ~ccount ~nd the other ~ccounts in the OU. Use third-p~rty routing softw~re to route tr~nsitive tr~ c between the VPCs.

 Correct ;;nswer: D
 C (71%)                             13%        Other

 Question #182
 ;; comp~ny is migr~ting ~n ~pplic~tion to ;;WS.  It w~nts to use fully m~n~ged services ~s much ~s possible during the migr~tion. The comp~ny needs to store l~rge import~nt documents within the ~pplic~tion with the following requirements: 1. The d~t~ must be highly dur~ble ~nd ~v~il~ble 2. The d~t~ must ~lw~ys be encrypted ~t rest ~nd in tr~nsit 3. The encryption key must be m~n~ged by the comp~ny ~nd rot~ted periodic~lly Which of the following solutions should the solutions ~rchitect recommend?
  ;;.  Deploy the stor~ge g~tew~y to ;;WS in  le g~tew~y mode. Use ;;m~zon  EBS volume encryption using ~n ;;WS  KMS key to encrypt the stor~ge g~tew~y volumes.
  B. Use ;;m~zon S3 with ~ bucket policy to enforce  HTTPS for connections to the bucket ~nd to enforce server-side encryption ~nd ;;WS  KMS for object encryption.
  C. Use ;;m~zon  Dyn~moDB with SSL to connect to  Dyn~moDB. Use ~n ;;WS  KMS key to encrypt  Dyn~moDB objects ~t rest.
  D.  Deploy inst~nces with ;;m~zon  EBS volumes ~tt~ched to store this d~t~. Use  EBS volume encryption using ~n ;;WS  KMS key to encrypt the d~t~.

 Correct ;;nswer: B
 B (100%)

 Question #183
 ;; comp~ny’s public ;;PI runs ~s t~sks on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS). The t~sks run on ;;WS  F~rg~te behind ~n ;;pplic~tion Lo~d  B~l~ncer (;;LB) ~nd ~re con gured with Service ;;uto Sc~ling for the t~sks b~sed on CPU utiliz~tion. This service h~s been running well for sever~l months. Recently, ;;PI perform~nce slowed down ~nd m~de the ~pplic~tion unus~ble. The comp~ny discovered th~t ~ signi c~nt number of SQL injection ~tt~cks h~d occurred ~g~inst the ;;PI ~nd th~t the ;;PI service h~d sc~led to its m~ximum ~mount. ;; solutions ~rchitect needs to implement ~ solution th~t prevents SQL injection ~tt~cks from re~ching the  ECS ;;PI service. The solution must ~llow legitim~te tr~ c through ~nd must m~ximize oper~tion~l e ciency. Which solution meets these requirements?
  ;;. Cre~te ~ new ;;WS W;;F web ;;CL to monitor the  HTTP requests ~nd  HTTPS requests th~t ~re forw~rded to the ;;LB in front of the  ECS t~sks.
  B. Cre~te ~ new ;;WS W;;F  Bot Control implement~tion. ;;dd ~ rule in the ;;WS W;;F  Bot Control m~n~ged rule group to monitor tr~ c ~nd ~llow only legitim~te tr~ c to the ;;LB in front of the  ECS t~sks.
  C. Cre~te ~ new ;;WS W;;F web ;;CL. ;;dd ~ new rule th~t blocks requests th~t m~tch the SQL d~t~b~se rule group. Set the web ;;CL to ~llow ~ll other tr~ c th~t does not m~tch those rules. ;;tt~ch the web ;;CL to the ;;LB in front of the  ECS t~sks.
  D. Cre~te ~ new ;;WS W;;F web ;;CL. Cre~te ~ new empty  IP set in ;;WS W;;F. ;;dd ~ new rule to the web ;;CL to block requests th~t origin~te from  IP ~ddresses in the new  IP set. Cre~te ~n ;;WS  L~mbd~ function th~t scr~pes the ;;PI logs for  IP ~ddresses th~t send SQL injection ~tt~cks, ~nd ~dd those  IP ~ddresses to the  IP set. ;;tt~ch the web ;;CL to the ;;LB in front of the  ECS t~sks.

 Correct ;;nswer: C
 C (100%)

 Question #184
 ;;n environment~l comp~ny is deploying sensors in m~jor cities throughout ~ country to me~sure ~ir qu~lity. The sensors connect to ;;WS  IoT Core to ingest timeseries d~t~ re~dings. The comp~ny stores the d~t~ in ;;m~zon  Dyn~moDB. For business continuity, the comp~ny must h~ve the ~bility to ingest ~nd store d~t~ in two ;;WS  Regions. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;m~zon  Route 53 ~li~s f~ilover routing policy with v~lues for ;;WS  IoT Core d~t~ endpoints in both  Regions  Migr~te d~t~ to ;;m~zon ;;uror~ glob~l t~bles.
  B. Cre~te ~ dom~in con gur~tion for ;;WS  IoT Core in e~ch  Region. Cre~te ~n ;;m~zon  Route 53 l~tency-b~sed routing policy. Use ;;WS  IoT Core d~t~ endpoints in both  Regions ~s v~lues.  Migr~te the d~t~ to ;;m~zon  MemoryDB for  Redis ~nd con gure cross-Region replic~tion.
  C. Cre~te ~ dom~in con gur~tion for ;;WS  IoT Core in e~ch  Region. Cre~te ~n ;;m~zon  Route 53 he~lth check th~t ev~lu~tes dom~in con gur~tion he~lth. Cre~te ~ f~ilover routing policy with v~lues for the dom~in n~me from the ;;WS  IoT Core dom~in con gur~tions. Upd~te the  Dyn~moDB t~ble to ~ glob~l t~ble.
  D. Cre~te ~n ;;m~zon  Route 53 l~tency-b~sed routing policy. Use ;;WS  IoT Core d~t~ endpoints in both  Regions ~s v~lues. Con gure Dyn~moDB stre~ms ~nd cross-Region d~t~ replic~tion.

 Correct ;;nswer: C
 C (100%)

 Question #185
 ;; comp~ny uses ;;WS Org~niz~tions for ~ multi-~ccount setup in the ;;WS Cloud. The comp~ny's  n~nce te~m h~s ~ d~t~ processing ~pplic~tion th~t uses ;;WS  L~mbd~ ~nd ;;m~zon  Dyn~moDB. The comp~ny's m~rketing te~m w~nts to ~ccess the d~t~ th~t is stored in the  Dyn~moDB t~ble. The  Dyn~moDB t~ble cont~ins con denti~l d~t~. The m~rketing te~m c~n h~ve ~ccess to only speci c ~ttributes of d~t~ in the  Dyn~moDB t~ble. The  n~nce te~m ~nd the m~rketing te~m h~ve sep~r~te ;;WS ~ccounts. Wh~t should ~ solutions ~rchitect do to provide the m~rketing te~m with the ~ppropri~te ~ccess to the  Dyn~moDB t~ble?
  ;;. Cre~te ~n SCP to gr~nt the m~rketing te~m's ;;WS ~ccount ~ccess to the speci c ~ttributes of the  Dyn~moDB t~ble. ;;tt~ch the SCP to the OU of the  n~nce te~m.
  B. Cre~te ~n  I;;M role in the  n~nce te~m's ~ccount by using  I;;M policy conditions for speci c  Dyn~moDB ~ttributes ( ne-gr~ined ~ccess control).  Est~blish trust with the m~rketing te~m's ~ccount.  In the m~rketing te~m's ~ccount, cre~te ~n  I;;M role th~t h~s permissions to ~ssume the  I;;M role in the  n~nce te~m's ~ccount.
  C. Cre~te ~ resource-b~sed  I;;M policy th~t includes conditions for speci c  Dyn~moDB ~ttributes ( ne-gr~ined ~ccess control). ;;tt~ch the policy to the  Dyn~moDB t~ble.  In the m~rketing te~m's ~ccount, cre~te ~n  I;;M role th~t h~s permissions to ~ccess the  Dyn~moDB t~ble in the  n~nce te~m's ~ccount.
  D. Cre~te ~n  I;;M role in the  n~nce te~m's ~ccount to ~ccess the  Dyn~moDB t~ble. Use ~n  I;;M permissions bound~ry to limit the ~ccess to the speci c ~ttributes.  In the m~rketing te~m's ~ccount, cre~te ~n  I;;M role th~t h~s permissions to ~ssume the  I;;M role in the  n~nce te~m's ~ccount.

 Correct ;;nswer: B
 B (94%)                                   6%

 Question #186
 ;; solutions ~rchitect is cre~ting ~n ~pplic~tion th~t stores objects in ~n ;;m~zon S3 bucket. The solutions ~rchitect must deploy the ~pplic~tion in two ;;WS  Regions th~t will be used simult~neously. The objects in the two S3 buckets must rem~in synchronized with e~ch other. Which combin~tion of steps will meet these requirements with the  LE;;ST oper~tion~l overhe~d? (Choose three.)
  ;;. Cre~te ~n S3  Multi-Region ;;ccess  Point Ch~nge the ~pplic~tion to refer to the  Multi-Region ;;ccess  Point
  B. Con gure two-w~y S3 Cross-Region  Replic~tion (CRR) between the two S3 buckets
  C.  Modify the ~pplic~tion to store objects in e~ch S3 bucket
  D. Cre~te ~n S3  Lifecycle rule for e~ch S3 bucket to copy objects from one S3 bucket to the other S3 bucket
  E.  En~ble S3 Versioning for e~ch S3 bucket
  F. Con gure ~n event noti c~tion for e~ch S3 bucket to invoke ~n ;;WS  L~mbd~ function to copy objects from one S3 bucket to the other S3 bucket

 Correct ;;nswer: ;;BE
 ;;BE (100%)

 Question #187
 ;; comp~ny h~s ~n  IoT pl~tform th~t runs in ~n on-premises environment. The pl~tform consists of ~ server th~t connects to  IoT devices by using the  MQTT protocol. The pl~tform collects telemetry d~t~ from the devices ~t le~st once every 5 minutes. The pl~tform ~lso stores device met~d~t~ in ~  MongoDB cluster. ;;n ~pplic~tion th~t is inst~lled on ~n on-premises m~chine runs periodic jobs to ~ggreg~te ~nd tr~nsform the telemetry ~nd device met~d~t~. The ~pplic~tion cre~tes reports th~t users view by using ~nother web ~pplic~tion th~t runs on the s~me on-premises m~chine. The periodic jobs t~ke 120-600 seconds to run.  However, the web ~pplic~tion is ~lw~ys running. The comp~ny is moving the pl~tform to ;;WS ~nd must reduce the oper~tion~l overhe~d of the st~ck. Which combin~tion of steps will meet these requirements with the  LE;;ST oper~tion~l overhe~d? (Choose three.)
  ;;. Use ;;WS  L~mbd~ functions to connect to the  IoT devices
  B. Con gure the  IoT devices to publish to ;;WS  IoT Core
  C. Write the met~d~t~ to ~ self-m~n~ged  MongoDB d~t~b~se on ~n ;;m~zon  EC2 inst~nce
  D. Write the met~d~t~ to ;;m~zon  DocumentDB (with  MongoDB comp~tibility)
  E. Use ;;WS Step  Functions st~te m~chines with ;;WS  L~mbd~ t~sks to prep~re the reports ~nd to write the reports to ;;m~zon S3. Use ;;m~zon CloudFront with ~n S3 origin to serve the reports
  F. Use ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster with ;;m~zon  EC2 inst~nces to prep~re the reports. Use ~n ingress controller in the  EKS cluster to serve the reports

 Correct ;;nswer: BDE
 BDE (100%)

 Question #188
 ;; glob~l m~nuf~cturing comp~ny pl~ns to migr~te the m~jority of its ~pplic~tions to ;;WS.  However, the comp~ny is concerned ~bout ~pplic~tions th~t need to rem~in within ~ speci c country or in the comp~ny's centr~l on-premises d~t~ center bec~use of d~t~ regul~tory requirements or requirements for l~tency of single-digit milliseconds. The comp~ny ~lso is concerned ~bout the ~pplic~tions th~t it hosts in some of its f~ctory sites, where limited network infr~structure exists. The comp~ny w~nts ~ consistent developer experience so th~t its developers c~n build ~pplic~tions once ~nd deploy on premises, in the cloud, or in ~ hybrid ~rchitecture. The developers must be ~ble to use the s~me tools, ;;PIs, ~nd services th~t ~re f~mili~r to them. Which solution will provide ~ consistent hybrid experience to meet these requirements?
  ;;.  Migr~te ~ll ~pplic~tions to the closest ;;WS  Region th~t is compli~nt. Set up ~n ;;WS  Direct Connect connection between the centr~l on- premises d~t~ center ~nd ;;WS.  Deploy ~  Direct Connect g~tew~y.
  B. Use ;;WS Snowb~ll  Edge Stor~ge Optimized devices for the ~pplic~tions th~t h~ve d~t~ regul~tory requirements or requirements for l~tency of single-digit milliseconds.  Ret~in the devices on premises.  Deploy ;;WS W~velength to host the worklo~ds in the f~ctory sites.
  C.  Inst~ll ;;WS Outposts for the ~pplic~tions th~t h~ve d~t~ regul~tory requirements or requirements for l~tency of single-digit milliseconds. Use ;;WS Snowb~ll  Edge Compute Optimized devices to host the worklo~ds in the f~ctory sites.
  D.  Migr~te the ~pplic~tions th~t h~ve d~t~ regul~tory requirements or requirements for l~tency of single-digit milliseconds to ~n ;;WS  Loc~l Zone.  Deploy ;;WS W~velength to host the worklo~ds in the f~ctory sites.

 Correct ;;nswer: C
 C (88%)                                   13%

 Question #189
 ;; comp~ny is upd~ting ~n ~pplic~tion th~t customers use to m~ke online orders. The number of ~tt~cks on the ~pplic~tion by b~d ~ctors h~s incre~sed recently. The comp~ny will host the upd~ted ~pplic~tion on ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster. The comp~ny will use ;;m~zon Dyn~moDB to store ~pplic~tion d~t~. ;; public ;;pplic~tion  Lo~d  B~l~ncer (;;LB) will provide end users with ~ccess to the ~pplic~tion. The comp~ny must prevent ~tt~cks ~nd ensure business continuity with minim~l service interruptions during ~n ongoing ~tt~ck. Which combin~tion of steps will meet these requirements  MOST cost-effectively? (Choose two.)
  ;;. Cre~te ~n ;;m~zon CloudFront distribution with the ;;LB ~s the origin. ;;dd ~ custom he~der ~nd r~ndom v~lue on the CloudFront dom~in. Con gure the ;;LB to condition~lly forw~rd tr~ c if the he~der ~nd v~lue m~tch.
  B.  Deploy the ~pplic~tion in two ;;WS  Regions. Con gure ;;m~zon  Route 53 to route to both  Regions with equ~l weight.
  C. Con gure ~uto sc~ling for ;;m~zon  ECS t~sks Cre~te ~  Dyn~moDB ;;cceler~tor (D;;X) cluster.
  D. Con gure ;;m~zon  El~stiC~che to reduce overhe~d on  Dyn~moDB.
  E.  Deploy ~n ;;WS W;;F web ;;CL th~t includes ~n ~ppropri~te rule group. ;;ssoci~te the web ;;CL with the ;;m~zon CloudFront distribution.

 Correct ;;nswer: ;;E
 ;;E (92%)                                    8%

 Question #190
 ;; comp~ny runs ~ web ~pplic~tion on ;;WS. The web ~pplic~tion delivers st~tic content from ~n ;;m~zon S3 bucket th~t is behind ~n ;;m~zon CloudFront distribution. The ~pplic~tion serves dyn~mic content by using ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t distributes requests to ~  eet of ;;m~zon  EC2 inst~nces in ;;uto Sc~ling groups. The ~pplic~tion uses ~ dom~in n~me setup in ;;m~zon  Route 53. Some users reported occ~sion~l issues when the users ~ttempted to ~ccess the website during pe~k hours. ;;n oper~tions te~m found th~t the ;;LB sometimes returned  HTTP 503 Service Un~v~il~ble errors. The comp~ny w~nts to displ~y ~ custom error mess~ge p~ge when these errors occur. The p~ge should be displ~yed immedi~tely for this error code. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Set up ~  Route 53 f~ilover routing policy. Con gure ~ he~lth check to determine the st~tus of the ;;LB endpoint ~nd to f~il over to the f~ilover S3 bucket endpoint.
  B. Cre~te ~ second CloudFront distribution ~nd ~n S3 st~tic website to host the custom error p~ge. Set up ~  Route 53 f~ilover routing policy. Use ~n ~ctive-p~ssive con gur~tion between the two distributions.
  C. Cre~te ~ CloudFront origin group th~t h~s two origins. Set the ;;LB endpoint ~s the prim~ry origin.  For the second~ry origin, set ~n S3 bucket th~t is con gured to host ~ st~tic website Set up origin f~ilover for the CloudFront distribution. Upd~te the S3 st~tic website to incorpor~te the custom error p~ge.
  D. Cre~te ~ CloudFront function th~t v~lid~tes e~ch  HTTP response code th~t the ;;LB returns. Cre~te ~n S3 st~tic website in ~n S3 bucket. Uplo~d the custom error p~ge to the S3 bucket ~s ~ f~ilover. Upd~te the function to re~d the S3 bucket ~nd to serve the error p~ge to the end users.

 Correct ;;nswer: C
 C (100%)

 Question #191
 ;; comp~ny is pl~nning to migr~te ~n ~pplic~tion to ;;WS. The ~pplic~tion runs ~s ~  Docker cont~iner ~nd uses ~n  NFS version 4  le sh~re. ;; solutions ~rchitect must design ~ secure ~nd sc~l~ble cont~inerized solution th~t does not require provisioning or m~n~gement of the underlying infr~structure. Which solution will meet these requirements?
  ;;.  Deploy the ~pplic~tion cont~iners by using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the  F~rg~te l~unch type. Use ;;m~zon El~stic  File System (;;m~zon  EFS) for sh~red stor~ge.  Reference the  EFS  le system  ID, cont~iner mount point, ~nd  EFS ~uthoriz~tion  I;;M role in the  ECS t~sk de nition.
  B.  Deploy the ~pplic~tion cont~iners by using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the  F~rg~te l~unch type. Use ;;m~zon  FSx for  Lustre for sh~red stor~ge.  Reference the  FSx for  Lustre  le system  ID, cont~iner mount point, ~nd  FSx for  Lustre ~uthoriz~tion  I;;M role in the  ECS t~sk de nition.
  C.  Deploy the ~pplic~tion cont~iners by using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the ;;m~zon  EC2 l~unch type ~nd ~uto sc~ling turned on. Use ;;m~zon  El~stic  File System (;;m~zon  EFS) for sh~red stor~ge.  Mount the  EFS  le system on the  ECS cont~iner inst~nces. ;;dd the  EFS ~uthoriz~tion  I;;M role to the  EC2 inst~nce pro le.
  D.  Deploy the ~pplic~tion cont~iners by using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the ;;m~zon  EC2 l~unch type ~nd ~uto sc~ling turned on. Use ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes with  Multi-;;tt~ch en~bled for sh~red stor~ge. ;;tt~ch the  EBS volumes to  ECS cont~iner inst~nces. ;;dd the  EBS ~uthoriz~tion  I;;M role to ~n  EC2 inst~nce pro le.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #192
 ;; comp~ny is running ~n ~pplic~tion in the ;;WS Cloud. The core business logic is running on ~ set of ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group. ;;n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) distributes tr~ c to the  EC2 inst~nces. ;;m~zon  Route 53 record ~pi.ex~mple.com is pointing to the ;;LB. The comp~ny's development te~m m~kes m~jor upd~tes to the business logic. The comp~ny h~s ~ rule th~t when ch~nges ~re deployed, only  10% of customers c~n receive the new logic during ~ testing window. ;; customer must use the s~me version of the business logic during the testing window. How should the comp~ny deploy the upd~tes to meet these requirements?
  ;;. Cre~te ~ second ;;LB, ~nd deploy the new logic to ~ set of  EC2 inst~nces in ~ new ;;uto Sc~ling group. Con gure the ;;LB to distribute tr~ c to the  EC2 inst~nces. Upd~te the  Route 53 record to use weighted routing, ~nd point the record to both of the ;;LBs.
  B. Cre~te ~ second t~rget group th~t is referenced by the ;;LDeploy the new logic to  EC2 inst~nces in this new t~rget group. Upd~te the ;;LB listener rule to use weighted t~rget groups. Con gure ;;LB t~rget group stickiness.
  C. Cre~te ~ new l~unch con gur~tion for the ;;uto Sc~ling group. Specify the l~unch con gur~tion to use the ;;utoSc~lingRollingUpd~te policy, ~nd set the  M~xB~tchSize option to  10.  Repl~ce the l~unch con gur~tion on the ;;uto Sc~ling group.  Deploy the ch~nges.
  D. Cre~te ~ second ;;uto Sc~ling group th~t is referenced by the ;;LB.  Deploy the new logic on ~ set of  EC2 inst~nces in this new ;;uto Sc~ling group. Ch~nge the ;;LB routing ~lgorithm to le~st outst~nding requests (LOR). Con gure ;;LB session stickiness.

 Correct ;;nswer: B
 B (100%)

 Question #193
 ;; l~rge educ~tion comp~ny recently introduced ;;m~zon Worksp~ces to provide ~ccess to intern~l ~pplic~tions ~cross multiple universities. The comp~ny is storing user pro les on ~n ;;m~zon  FSx for Windows  File Server  le system. The  le system is con gured with ~  DNS ~li~s ~nd is connected to ~ self-m~n~ged ;;ctive  Directory. ;;s more users begin to use the Worksp~ces, login time incre~ses to un~ccept~ble levels. ;;n investig~tion reve~ls ~ degr~d~tion in perform~nce of the  le system. The comp~ny cre~ted the  le system on  HDD stor~ge with ~ throughput of  16  MBps. ;; solutions ~rchitect must improve the perform~nce of the  le system during ~ de ned m~inten~nce window. Wh~t should the solutions ~rchitect do to meet these requirements with the  LE;;ST ~dministr~tive effort?
  ;;. Use ;;WS  B~ckup to cre~te ~ point-in-time b~ckup of the  le system.  Restore the b~ckup to ~ new  FSx for Windows  File Server  le system. Select SSD ~s the stor~ge type. Select 32  MBps ~s the throughput c~p~city. When the b~ckup ~nd restore process is completed, ~djust the DNS ~li~s ~ccordingly.  Delete the origin~l  le system.
  B.  Disconnect users from the  le system.  In the ;;m~zon  FSx console, upd~te the throughput c~p~city to 32  MBps. Upd~te the stor~ge type to SSD.  Reconnect users to the  le system.
  C.  Deploy ~n ;;WS  D~t~Sync ~gent onto ~ new ;;m~zon  EC2 inst~nce. Cre~te ~ t~sk. Con gure the existing  le system ~s the source loc~tion. Con gure ~ new  FSx for Windows  File Server  le system with SSD stor~ge ~nd 32  MBps of throughput ~s the t~rget loc~tion. Schedule the t~sk. When the t~sk is completed, ~djust the  DNS ~li~s ~ccordingly.  Delete the origin~l  le system.
  D.  En~ble sh~dow copies on the existing  le system by using ~ Windows  PowerShell comm~nd. Schedule the sh~dow copy job to cre~te ~ point-in-time b~ckup of the  le system. Choose to restore previous versions. Cre~te ~ new  FSx for Windows  File Server  le system with SSD stor~ge ~nd 32  MBps of throughput. When the copy job is completed, ~djust the  DNS ~li~s.  Delete the origin~l  le system.

 Correct ;;nswer: ;;
 ;; (50%)                                 B (50%)

 Question #194
 ;; comp~ny hosts ~n ~pplic~tion on ;;WS. The ~pplic~tion re~ds ~nd writes objects th~t ~re stored in ~ single ;;m~zon S3 bucket. The comp~ny must modify the ~pplic~tion to deploy the ~pplic~tion in two ;;WS  Regions. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Set up ~n ;;m~zon CloudFront distribution with the S3 bucket ~s ~n origin.  Deploy the ~pplic~tion to ~ second  Region  Modify the ~pplic~tion to use the CloudFront distribution. Use ;;WS Glob~l ;;cceler~tor to ~ccess the d~t~ in the S3 bucket.
  B. Cre~te ~ new S3 bucket in ~ second  Region. Set up bidirection~l S3 Cross-Region  Replic~tion (CRR) between the origin~l S3 bucket ~nd the new S3 bucket. Con gure ~n S3  Multi-Region ;;ccess  Point th~t uses both S3 buckets.  Deploy ~ modi ed ~pplic~tion to both  Regions.
  C. Cre~te ~ new S3 bucket in ~ second  Region  Deploy the ~pplic~tion in the second  Region. Con gure the ~pplic~tion to use the new S3 bucket. Set up S3 Cross-Region  Replic~tion (CRR) from the origin~l S3 bucket to the new S3 bucket.
  D. Set up ~n S3 g~tew~y endpoint with the S3 bucket ~s ~n origin.  Deploy the ~pplic~tion to ~ second  Region.  Modify the ~pplic~tion to use the new S3 g~tew~y endpoint. Use S3  Intelligent-Tiering on the S3 bucket.

 Correct ;;nswer: B
 B (82%)                                  C (18%)

 Question #195
 ;;n online g~ming comp~ny needs to rehost its g~ming pl~tform on ;;WS. The comp~ny's g~ming ~pplic~tion requires high perform~nce computing (HPC) processing ~nd h~s ~ le~derbo~rd th~t ch~nges frequently. ;;n Ubuntu inst~nce th~t is optimized for compute gener~tion hosts ~  Node.js ~pplic~tion for g~me displ~y. G~me st~te is tr~cked in ~n on-premises  Redis inst~nce. The comp~ny needs ~ migr~tion str~tegy th~t optimizes ~pplic~tion perform~nce. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;uto Sc~ling group of m5.l~rge ;;m~zon  EC2 Spot  Inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Use ~n ;;m~zon  El~stlC~che for  Redis cluster to m~int~in the le~derbo~rd.
  B. Cre~te ~n ;;uto Sc~ling group of c5.l~rge ;;m~zon  EC2 Spot  Inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Use ~n ;;m~zon OpenSe~rch Service cluster to m~int~in the le~derbo~rd.
  C. Cre~te ~n ;;uto Sc~ling group of c5.l~rge ;;m~zon  EC2 On-Dem~nd  Inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Use ~n ;;m~zon El~stiC~che for  Redis cluster to m~int~in the le~derbo~rd.
  D. Cre~te ~n ;;uto Sc~ling group of m5.l~rge ;;m~zon  EC2 On-Dem~nd  Inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Use ~n ;;m~zon Dyn~moDB t~ble to m~int~in the le~derbo~rd.

 Correct ;;nswer: C
 C (100%)

 Question #196
 ;; solutions ~rchitect is designing ~n ~pplic~tion to ~ccept timesheet entries from employees on their mobile devices. Timesheets will be submitted weekly, with most of the submissions occurring on  Frid~y. The d~t~ must be stored in ~ form~t th~t ~llows p~yroll ~dministr~tors to run monthly reports. The infr~structure must be highly ~v~il~ble ~nd sc~le to m~tch the r~te of incoming d~t~ ~nd reporting requests. Which combin~tion of steps meets these requirements while minimizing oper~tion~l overhe~d? (Choose two.)
  ;;.  Deploy the ~pplic~tion to ;;m~zon  EC2 On-Dem~nd  Inst~nces with lo~d b~l~ncing ~cross multiple ;;v~il~bility Zones. Use scheduled ;;m~zon  EC2 ;;uto Sc~ling to ~dd c~p~city before the high volume of submissions on  Frid~ys.
  B.  Deploy the ~pplic~tion in ~ cont~iner using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with lo~d b~l~ncing ~cross multiple ;;v~il~bility Zones. Use scheduled Service ;;uto Sc~ling to ~dd c~p~city before the high volume of submissions on  Frid~ys.
  C.  Deploy the ~pplic~tion front end to ~n ;;m~zon S3 bucket served by ;;m~zon CloudFront.  Deploy the ~pplic~tion b~ckend using ;;m~zon ;;PI G~tew~y with ~n ;;WS  L~mbd~ proxy integr~tion.
  D. Store the timesheet submission d~t~ in ;;m~zon  Redshift. Use ;;m~zon QuickSight to gener~te the reports using ;;m~zon  Redshift ~s the d~t~ source.
  E. Store the timesheet submission d~t~ in ;;m~zon S3. Use ;;m~zon ;;then~ ~nd ;;m~zon QuickSight to gener~te the reports using ;;m~zon S3 ~s the d~t~ source.

 Correct ;;nswer: BE
 CE (58%)                       BE (18%)       13%       8%

 Question #197
 ;; comp~ny is storing sensitive d~t~ in ~n ;;m~zon S3 bucket. The comp~ny must log ~ll ~ctivities for objects in the S3 bucket ~nd must keep the logs for 5 ye~rs. The comp~ny's security te~m ~lso must receive ~n em~il noti c~tion every time there is ~n ~ttempt to delete d~t~ in the S3 bucket. Which combin~tion of steps will meet these requirements  MOST cost-effectively? (Choose three.)
  ;;. Con gure ;;WS CloudTr~il to log S3 d~t~ events.
  B. Con gure S3 server ~ccess logging for the S3 bucket.
  C. Con gure ;;m~zon S3 to send object deletion events to ;;m~zon Simple  Em~il Service (;;m~zon SES).
  D. Con gure ;;m~zon S3 to send object deletion events to ~n ;;m~zon  EventBridge event bus th~t publishes to ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic.
  E. Con gure ;;m~zon S3 to send the logs to ;;m~zon Timestre~m with d~t~ stor~ge tiering.
  F. Con gure ~ new S3 bucket to store the logs with ~n S3  Lifecycle policy.

 Correct ;;nswer: ;;DF
 ;;DF (51%)                                BDF (48%)

 Question #198
 ;; comp~ny is building ~ hybrid environment th~t includes servers in ~n on-premises d~t~ center ~nd in the ;;WS Cloud. The comp~ny h~s deployed ;;m~zon  EC2 inst~nces in three VPCs.  E~ch VPC is in ~ different ;;WS  Region. The comp~ny h~s est~blished ~n ;;WS  Direct. Connect connection to the d~t~ center from the  Region th~t is closest to the d~t~ center. The comp~ny needs the servers in the on-premises d~t~ center to h~ve ~ccess to the  EC2 inst~nces in ~ll three VPCs. The servers in the on- premises d~t~ center ~lso must h~ve ~ccess to ;;WS public services. Which combin~tion of steps will meet these requirements with the  LE;;ST cost? (Choose two.)
  ;;. Cre~te ~  Direct Connect g~tew~y in the  Region th~t is closest to the d~t~ center. ;;tt~ch the  Direct Connect connection to the  Direct Connect g~tew~y. Use the  Direct Connect g~tew~y to connect the VPCs in the other two  Regions.
  B. Set up ~ddition~l  Direct Connect connections from the on-premises d~t~ center to the other two  Regions.
  C. Cre~te ~ priv~te VIF.  Est~blish ~n ;;WS Site-to-Site VPN connection over the priv~te VIF to the VPCs in the other two  Regions.
  D. Cre~te ~ public VIF.  Est~blish ~n ;;WS Site-to-Site VPN connection over the public VIF to the VPCs in the other two  Regions.
  E. Use VPC peering to est~blish ~ connection between the VPCs ~cross the  Regions Cre~te ~ priv~te VIF with the existing  Direct Connect connection to connect to the peered VPCs.

 Correct ;;nswer: ;;D
 ;;D (100%)

 Question #199
 ;; comp~ny is using ~n org~niz~tion in ;;WS Org~niz~tions to m~n~ge hundreds of ;;WS ~ccounts. ;; solutions ~rchitect is working on ~ solution to provide b~seline protection for the Open Web ;;pplic~tion Security  Project (OW;;SP) top  10 web ~pplic~tion vulner~bilities. The solutions ~rchitect is using ;;WS W;;F for ~ll existing ~nd new ;;m~zon CloudFront distributions th~t ~re deployed within the org~niz~tion. Which combin~tion of steps should the solutions ~rchitect t~ke to provide the b~seline protection? (Choose three.)
  ;;.  En~ble ;;WS Con g in ~ll ~ccounts
  B.  En~ble ;;m~zon Gu~rdDuty in ~ll ~ccounts
  C.  En~ble ~ll fe~tures for the org~niz~tion
  D. Use ;;WS  Firew~ll  M~n~ger to deploy ;;WS W;;F rules in ~ll ~ccounts for ~ll CloudFront distributions
  E. Use ;;WS Shield ;;dv~nced to deploy ;;WS W;;F rules in ~ll ~ccounts for ~ll CloudFront distributions
  F. Use ;;WS Security  Hub to deploy ;;WS W;;F rules in ~ll ~ccounts for ~ll CloudFront distributions

 Correct ;;nswer: CDF
 ;;CD (69%)                         7%    7%       Other

 Question #200
 ;; solutions ~rchitect h~s implemented ~ S;;ML 2.0 feder~ted identity solution with their comp~ny's on-premises identity provider (IdP) to ~uthentic~te users' ~ccess to the ;;WS environment. When the solutions ~rchitect tests ~uthentic~tion through the feder~ted identity web port~l, ~ccess to the ;;WS environment is gr~nted.  However, when test users ~ttempt to ~uthentic~te through the feder~ted identity web port~l, they ~re not ~ble to ~ccess the ;;WS environment. Which items should the solutions ~rchitect check to ensure identity feder~tion is properly con gured? (Choose three.)
  ;;. The  I;;M user's permissions policy h~s ~llowed the use of S;;ML feder~tion for th~t user.
  B. The  I;;M roles cre~ted for the feder~ted users' or feder~ted groups' trust policy h~ve set the S;;ML provider ~s the princip~l.
  B. Test users ~re not in the ;;WSFeder~tedUsers group in the comp~ny's  IdP.
  C. The web port~l c~lls the ;;WS STS ;;ssumeRoleWithS;;ML ;;PI with the ;;RN of the S;;ML provider, the ;;RN of the  I;;M role, ~nd the S;;ML ~ssertion from  IdP.
  D. The on-premises  IdP's  DNS hostn~me is re~ch~ble from the ;;WS environment VPCs.
  E. The comp~ny's  IdP de nes S;;ML ~ssertions th~t properly m~p users or groups.  In the comp~ny to  I;;M roles with ~ppropri~te permissions.

 Correct ;;nswer: BDF
 BCE (60%)                         B (20%)         BD (20%)

 Question #201
 ;; solutions ~rchitect needs to improve ~n ~pplic~tion th~t is hosted in the ;;WS Cloud. The ~pplic~tion uses ~n ;;m~zon ;;uror~  MySQL  DB inst~nce th~t is experiencing overlo~ded connections.  Most of the ~pplic~tion’s oper~tions insert records into the d~t~b~se. The ~pplic~tion currently stores credenti~ls in ~ text-b~sed con gur~tion  le. The solutions ~rchitect needs to implement ~ solution so th~t the ~pplic~tion c~n h~ndle the current connection lo~d. The solution must keep the credenti~ls secure ~nd must provide the ~bility to rot~te the credenti~ls ~utom~tic~lly on ~ regul~r b~sis. Which solution will meet these requirements?
  ;;.  Deploy ~n ;;m~zon  RDS  Proxy l~yer.  In front of the  DB inst~nce. Store the connection credenti~ls ~s ~ secret in ;;WS Secrets  M~n~ger.
  B.  Deploy ~n ;;m~zon  RDS  Proxy l~yer in front of the  DB inst~nce. Store the connection credenti~ls in ;;WS Systems  M~n~ger  P~r~meter Store
  C. Cre~te ~n ;;uror~  Replic~. Store the connection credenti~ls ~s ~ secret in ;;WS Secrets  M~n~ger
  D. Cre~te ~n ;;uror~  Replic~. Store the connection credenti~ls in ;;WS Systems  M~n~ger  P~r~meter Store.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #202
 ;; comp~ny needs to build ~ dis~ster recovery (DR) solution for its ecommerce website. The web ~pplic~tion is hosted on ~  eet of t3.l~rge ;;m~zon  EC2 inst~nces ~nd uses ~n ;;m~zon  RDS for  MySQL  DB inst~nce. The  EC2 inst~nces ~re in ~n ;;uto Sc~ling group th~t extends ~cross multiple ;;v~il~bility Zones. In the event of ~ dis~ster, the web ~pplic~tion must f~il over to the second~ry environment with ~n  RPO of 30 seconds ~nd ~n  RTO of  10 minutes. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Use infr~structure ~s code (I~C) to provision the new infr~structure in the  DR  Region. Cre~te ~ cross-Region re~d replic~ for the  DB inst~nce. Set up ~ b~ckup pl~n in ;;WS  B~ckup to cre~te cross-Region b~ckups for the  EC2 inst~nces ~nd the  DB inst~nce. Cre~te ~ cron expression to b~ck up the  EC2 inst~nces ~nd the  DB inst~nce every 30 seconds to the  DR  Region.  Recover the  EC2 inst~nces from the l~test EC2 b~ckup. Use ~n ;;m~zon  Route 53 geoloc~tion routing policy to ~utom~tic~lly f~il over to the  DR  Region in the event of ~ dis~ster.
  B. Use infr~structure ~s code (I~C) to provision the new infr~structure in the  DR  Region. Cre~te ~ cross-Region re~d replic~ for the  DB inst~nce. Set up ;;WS  El~stic  Dis~ster  Recovery to continuously replic~te the  EC2 inst~nces to the  DR  Region.  Run the  EC2 inst~nces ~t the minimum c~p~city in the  DR  Region. Use ~n ;;m~zon  Route 53 f~ilover routing policy to ~utom~tic~lly f~il over to the  DR  Region in the event of ~ dis~ster.  Incre~se the desired c~p~city of the ;;uto Sc~ling group.
  C. Set up ~ b~ckup pl~n in ;;WS  B~ckup to cre~te cross-Region b~ckups for the  EC2 inst~nces ~nd the  DB inst~nce. Cre~te ~ cron expression to b~ck up the  EC2 inst~nces ~nd the  DB inst~nce every 30 seconds to the  DR  Region. Use infr~structure ~s code (I~C) to provision the new infr~structure in the  DR  Region.  M~nu~lly restore the b~cked-up d~t~ on new inst~nces. Use ~n ;;m~zon  Route 53 simple routing policy to ~utom~tic~lly f~il over to the  DR  Region in the event of ~ dis~ster.
  D. Use infr~structure ~s code (I~C) to provision the new infr~structure in the  DR  Region. Cre~te ~n ;;m~zon ;;uror~ glob~l d~t~b~se. Set up ;;WS  El~stic  Dis~ster  Recovery to continuously replic~te the  EC2 inst~nces to the  DR  Region.  Run the ;;uto Sc~ling group of  EC2 inst~nces ~t full c~p~city in the  DR  Region. Use ~n ;;m~zon  Route 53 f~ilover routing policy to ~utom~tic~lly f~il over to the  DR  Region in the event of ~ dis~ster.

 Correct ;;nswer: B
 B (87%)                                    7%

 Question #203
 ;; comp~ny is pl~nning ~ one-time migr~tion of ~n on-premises  MySQL d~t~b~se to ;;m~zon ;;uror~  MySQL in the us-e~st-1  Region. The comp~ny's current internet connection h~s limited b~ndwidth. The on-premises  MySQL d~t~b~se is 60 TB in size. The comp~ny estim~tes th~t it will t~ke ~ month to tr~nsfer the d~t~ to ;;WS over the current internet connection. The comp~ny needs ~ migr~tion solution th~t will migr~te the d~t~b~se more quickly. Which solution will migr~te the d~t~b~se in the  LE;;ST ~mount of time?
  ;;.  Request ~  1 Gbps ;;WS  Direct Connect connection between the on-premises d~t~ center ~nd ;;WS. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to migr~te the on-premises  MySQL d~t~b~se to ;;uror~  MySQL.
  B. Use ;;WS  D~t~Sync with the current internet connection to ~cceler~te the d~t~ tr~nsfer between the on-premises d~t~ center ~nd ;;WS. Use ;;WS ;;pplic~tion  Migr~tion Service to migr~te the on-premises  MySQL d~t~b~se to ;;uror~  MySQL.
  C. Order ~n ;;WS Snowb~ll  Edge device.  Lo~d the d~t~ into ~n ;;m~zon S3 bucket by using the S3 interf~ce. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to migr~te the d~t~ from ;;m~zon S3 to ;;uror~  MySQL.
  D. Order ~n ;;WS Snowb~ll device.  Lo~d the d~t~ into ~n ;;m~zon S3 bucket by using the S3 ;;d~pter for Snowb~ll. Use ;;WS ;;pplic~tion Migr~tion Service to migr~te the d~t~ from ;;m~zon S3 to ;;uror~  MySQL.

 Correct ;;nswer: C
 C (95%)                                    5%

 Question #204
 ;; comp~ny h~s ~n ~pplic~tion in the ;;WS Cloud. The ~pplic~tion runs on ~  eet of 20 ;;m~zon  EC2 inst~nces. The  EC2 inst~nces ~re persistent ~nd store d~t~ on multiple ~tt~ched ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes. The comp~ny must m~int~in b~ckups in ~ sep~r~te ;;WS  Region. The comp~ny must be ~ble to recover the  EC2 inst~nces ~nd their con gur~tion within  1 business d~y, with loss of no more th~n  1 d~y's worth of d~t~. The comp~ny h~s limited st~ff ~nd needs ~ b~ckup solution th~t optimizes oper~tion~l e ciency ~nd cost. The comp~ny ~lre~dy h~s cre~ted ~n ;;WS CloudForm~tion templ~te th~t c~n deploy the required network con gur~tion in ~ second~ry  Region. Which solution will meet these requirements?
  ;;. Cre~te ~ second CloudForm~tion templ~te th~t c~n recre~te the  EC2 inst~nces in the second~ry  Region.  Run d~ily multivolume sn~pshots by using ;;WS Systems  M~n~ger ;;utom~tion runbooks. Copy the sn~pshots to the second~ry  Region.  In the event of ~ f~ilure l~unch the CloudForm~tion templ~tes, restore the  EBS volumes from sn~pshots, ~nd tr~nsfer us~ge to the second~ry  Region.
  B. Use ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM) to cre~te d~ily multivolume sn~pshots of the  EBS volumes.  In the event of ~ f~ilure, l~unch the CloudForm~tion templ~te ~nd use ;;m~zon  DLM to restore the  EBS volumes ~nd tr~nsfer us~ge to the second~ry  Region.
  C. Use ;;WS  B~ckup to cre~te ~ scheduled d~ily b~ckup pl~n for the  EC2 inst~nces. Con gure the b~ckup t~sk to copy the b~ckups to ~ v~ult in the second~ry  Region.  In the event of ~ f~ilure, l~unch the CloudForm~tion templ~te, restore the inst~nce volumes ~nd con gur~tions from the b~ckup v~ult, ~nd tr~nsfer us~ge to the second~ry  Region.
  D.  Deploy  EC2 inst~nces of the s~me size ~nd con gur~tion to the second~ry  Region. Con gure ;;WS  D~t~Sync d~ily to copy d~t~ from the prim~ry  Region to the second~ry  Region.  In the event of ~ f~ilure, l~unch the CloudForm~tion templ~te ~nd tr~nsfer us~ge to the second~ry Region.

 Correct ;;nswer: C
 C (81%)                                  B (19%)

 Question #205
 ;; comp~ny is designing ~ new website th~t hosts st~tic content. The website will give users the ~bility to uplo~d ~nd downlo~d l~rge  les. ;;ccording to comp~ny requirements, ~ll d~t~ must be encrypted in tr~nsit ~nd ~t rest. ;; solutions ~rchitect is building the solution by using ;;m~zon S3 ~nd ;;m~zon CloudFront. Which combin~tion of steps will meet the encryption requirements? (Choose three.)
  ;;. Turn on S3 server-side encryption for the S3 bucket th~t the web ~pplic~tion uses.
  B. ;;dd ~ policy ~ttribute of "~ws:SecureTr~nsport": "true" for re~d ~nd write oper~tions in the S3 ;;CLs.
  C. Cre~te ~ bucket policy th~t denies ~ny unencrypted oper~tions in the S3 bucket th~t the web ~pplic~tion uses.
  D. Con gure encryption ~t rest on CloudFront by using server-side encryption with ;;WS  KMS keys (SSE-KMS).
  E. Con gure redirection of  HTTP requests to  HTTPS requests in CloudFront.
  F. Use the  RequireSSL option in the cre~tion of presigned URLs for the S3 bucket th~t the web ~pplic~tion uses.

 Correct ;;nswer: ;;CE
 ;;CE (95%)                                   5%

 Question #206
 ;; comp~ny is implementing ~ serverless ~rchitecture by using ;;WS  L~mbd~ functions th~t need to ~ccess ~  Microsoft SQL Server  DB inst~nce on ;;m~zon  RDS. The comp~ny h~s sep~r~te environments for development ~nd production, including ~ clone of the d~t~b~se system. The comp~ny's developers ~re ~llowed to ~ccess the credenti~ls for the development d~t~b~se.  However, the credenti~ls for the production d~t~b~se must be encrypted with ~ key th~t only members of the  IT security te~m's  I;;M user group c~n ~ccess. This key must be rot~ted on ~ regul~r b~sis. Wh~t should ~ solutions ~rchitect do in the production environment to meet these requirements?
  ;;. Store the d~t~b~se credenti~ls in ;;WS Systems  M~n~ger  P~r~meter Store by using ~ SecureString p~r~meter th~t is encrypted by ~n ;;WS Key  M~n~gement Service (;;WS  KMS) customer m~n~ged key. ;;tt~ch ~ role to e~ch  L~mbd~ function to provide ~ccess to the SecureString p~r~meter.  Restrict ~ccess to the SecureString p~r~meter ~nd the customer m~n~ged key so th~t only the  IT security te~m c~n ~ccess the p~r~meter ~nd the key.
  B.  Encrypt the d~t~b~se credenti~ls by using the ;;WS  Key  M~n~gement Service (;;WS  KMS) def~ult  L~mbd~ key. Store the credenti~ls in the environment v~ri~bles of e~ch  L~mbd~ function.  Lo~d the credenti~ls from the environment v~ri~bles in the  L~mbd~ code.  Restrict ~ccess to the  KMS key so th~t only the  IT security te~m c~n ~ccess the key.
  C. Store the d~t~b~se credenti~ls in the environment v~ri~bles of e~ch  L~mbd~ function.  Encrypt the environment v~ri~bles by using ~n ;;WS Key  M~n~gement Service (;;WS  KMS) customer m~n~ged key.  Restrict ~ccess to the customer m~n~ged key so th~t only the  IT security te~m c~n ~ccess the key.
  D. Store the d~t~b~se credenti~ls in ;;WS Secrets  M~n~ger ~s ~ secret th~t is ~ssoci~ted with ~n ;;WS  Key  M~n~gement Service (;;WS  KMS) customer m~n~ged key. ;;tt~ch ~ role to e~ch  L~mbd~ function to provide ~ccess to the secret.  Restrict ~ccess to the secret ~nd the customer m~n~ged key so th~t only the  IT security te~m c~n ~ccess the secret ~nd the key.

 Correct ;;nswer: D
 D (76%)                                  ;; (24%)

 Question #207
 ;;n online ret~il comp~ny is migr~ting its leg~cy on-premises .NET ~pplic~tion to ;;WS. The ~pplic~tion runs on lo~d-b~l~nced frontend web servers, lo~d-b~l~nced ~pplic~tion servers, ~nd ~  Microsoft SQL Server d~t~b~se. The comp~ny w~nts to use ;;WS m~n~ged services where possible ~nd does not w~nt to rewrite the ~pplic~tion. ;; solutions ~rchitect needs to implement ~ solution to resolve sc~ling issues ~nd minimize licensing costs ~s the ~pplic~tion sc~les. Which solution will meet these requirements  MOST cost-effectively?
  ;;.  Deploy ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group behind ~n ;;pplic~tion  Lo~d  B~l~ncer for the web tier ~nd for the ~pplic~tion tier. Use ;;m~zon ;;uror~  PostgreSQL with  B~bel sh turned on to repl~tform the SQL Server d~t~b~se.
  B. Cre~te im~ges of ~ll the servers by using ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS).  Deploy ;;m~zon  EC2 inst~nces th~t ~re b~sed on the on-premises imports.  Deploy the inst~nces in ~n ;;uto Sc~ling group behind ~  Network  Lo~d  B~l~ncer for the web tier ~nd for the ~pplic~tion tier. Use ;;m~zon  Dyn~moDB ~s the d~t~b~se tier.
  C. Cont~inerize the web frontend tier ~nd the ~pplic~tion tier.  Provision ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster. Cre~te ~n ;;uto Sc~ling group behind ~  Network  Lo~d  B~l~ncer for the web tier ~nd for the ~pplic~tion tier. Use ;;m~zon  RDS for SQL Server to host the d~t~b~se.
  D. Sep~r~te the ~pplic~tion functions into ;;WS  L~mbd~ functions. Use ;;m~zon ;;PI G~tew~y for the web frontend tier ~nd the ~pplic~tion tier. Migr~te the d~t~ to ;;m~zon S3. Use ;;m~zon ;;then~ to query the d~t~.

 Correct ;;nswer: ;;
 ;; (85%)                                  C (15%)

 Question #208
 ;; softw~re-~s-~-service (S~~S) provider exposes ;;PIs through ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The ;;LB connects to ~n ;;m~zon  El~stic Kubernetes Service (;;m~zon  EKS) cluster th~t is deployed in the us-e~st-1  Region. The exposed ;;PIs cont~in us~ge of ~ few non-st~nd~rd  REST methods:  LINK, UNLINK,  LOCK, ~nd UNLOCK. Users outside the United St~tes ~re reporting long ~nd inconsistent response times for these ;;PIs. ;; solutions ~rchitect needs to resolve this problem with ~ solution th~t minimizes oper~tion~l overhe~d. Which solution meets these requirements?
  ;;. ;;dd ~n ;;m~zon CloudFront distribution. Con gure the ;;LB ~s the origin.
  B. ;;dd ~n ;;m~zon ;;PI G~tew~y edge-optimized ;;PI endpoint to expose the ;;PIs. Con gure the ;;LB ~s the t~rget.
  C. ;;dd ~n ~cceler~tor in ;;WS Glob~l ;;cceler~tor. Con gure the ;;LB ~s the origin.
  D.  Deploy the ;;PIs to two ~ddition~l ;;WS  Regions: eu-west-1 ~nd ~p-southe~st-2. ;;dd l~tency-b~sed routing records in ;;m~zon  Route 53.

 Correct ;;nswer: C
 C (71%)                                 B (26%)

 Question #209
 ;; comp~ny runs ~n  IoT ~pplic~tion in the ;;WS Cloud. The comp~ny h~s millions of sensors th~t collect d~t~ from houses in the United St~tes. The sensors use the  MQTT protocol to connect ~nd send d~t~ to ~ custom  MQTT broker. The  MQTT broker stores the d~t~ on ~ single ;;m~zon  EC2 inst~nce. The sensors connect to the broker through the dom~in n~med iot.ex~mple.com. The comp~ny uses ;;m~zon  Route 53 ~s its  DNS service. The comp~ny stores the d~t~ in ;;m~zon  Dyn~moDB. On sever~l occ~sions, the ~mount of d~t~ h~s overlo~ded the  MQTT broker ~nd h~s resulted in lost sensor d~t~. The comp~ny must improve the reli~bility of the solution. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd ~n ;;uto Sc~ling group for the  MQTT broker. Use the ;;uto Sc~ling group ~s the t~rget for the ;;LB. Upd~te the  DNS record in  Route 53 to ~n ~li~s record.  Point the ~li~s record to the ;;LB. Use the  MQTT broker to store the d~t~.
  B. Set up ;;WS  IoT Core to receive the sensor d~t~. Cre~te ~nd con gure ~ custom dom~in to connect to ;;WS  IoT Core. Upd~te the  DNS record in  Route 53 to point to the ;;WS  IoT Core  D~t~-;;TS endpoint. Con gure ~n ;;WS  IoT rule to store the d~t~.
  C. Cre~te ~  Network  Lo~d  B~l~ncer (NLB). Set the  MQTT broker ~s the t~rget. Cre~te ~n ;;WS Glob~l ;;cceler~tor ~cceler~tor. Set the  NLB ~s the endpoint for the ~cceler~tor. Upd~te the  DNS record in  Route 53 to ~ multiv~lue ~nswer record. Set the Glob~l ;;cceler~tor  IP ~ddresses ~s v~lues. Use the  MQTT broker to store the d~t~.
  D. Set up ;;WS  IoT Greengr~ss to receive the sensor d~t~. Upd~te the  DNS record in  Route 53 to point to the ;;WS  IoT Greengr~ss endpoint. Con gure ~n ;;WS  IoT rule to invoke ~n ;;WS  L~mbd~ function to store the d~t~.

 Correct ;;nswer: C
 B (100%)

 Question #210
 ;; comp~ny h~s  Linux-b~sed ;;m~zon  EC2 inst~nces. Users must ~ccess the inst~nces by using SSH with  EC2 SSH key p~irs.  E~ch m~chine requires ~ unique  EC2 key p~ir. The comp~ny w~nts to implement ~ key rot~tion policy th~t will, upon request, ~utom~tic~lly rot~te ~ll the  EC2 key p~irs ~nd keep the keys in ~ securely encrypted pl~ce. The comp~ny will ~ccept less th~n  1 minute of downtime during key rot~tion. Which solution will meet these requirements?
  ;;. Store ~ll the keys in ;;WS Secrets  M~n~ger.  De ne ~ Secrets  M~n~ger rot~tion schedule to invoke ~n ;;WS  L~mbd~ function to gener~te new key p~irs.  Repl~ce public keys on  EC2 inst~nces. Upd~te the priv~te keys in Secrets  M~n~ger.
  B. Store ~ll the keys in  P~r~meter Store, ~ c~p~bility of ;;WS Systems  M~n~ger, ~s ~ string.  De ne ~ Systems  M~n~ger m~inten~nce window to invoke ~n ;;WS  L~mbd~ function to gener~te new key p~irs.  Repl~ce public keys on  EC2 inst~nces. Upd~te the priv~te keys in  P~r~meter Store.
  C.  Import the  EC2 key p~irs into ;;WS  Key  M~n~gement Service (;;WS  KMS). Con gure ~utom~tic key rot~tion for these key p~irs. Cre~te ~n ;;m~zon  EventBridge scheduled rule to invoke ~n ;;WS  L~mbd~ function to initi~te the key rot~tion in ;;WS  KMS.
  D. ;;dd ~ll the  EC2 inst~nces to  Fleet  M~n~ger, ~ c~p~bility of ;;WS Systems  M~n~ger.  De ne ~ Systems  M~n~ger m~inten~nce window to issue ~ Systems  M~n~ger  Run Comm~nd document to gener~te new key p~irs ~nd to rot~te public keys to ~ll the inst~nces in  Fleet  M~n~ger.

 Correct ;;nswer: ;;
 ;; (76%)                                 D (24%)

 Question #211
 ;; comp~ny w~nts to migr~te to ;;WS. The comp~ny is running thous~nds of VMs in ~ VMw~re  ESXi environment. The comp~ny h~s no con gur~tion m~n~gement d~t~b~se ~nd h~s little knowledge ~bout the utiliz~tion of the VMw~re portfolio. ;; solutions ~rchitect must provide the comp~ny with ~n ~ccur~te inventory so th~t the comp~ny c~n pl~n for ~ cost-effective migr~tion. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Use ;;WS Systems  M~n~ger  P~tch  M~n~ger to deploy  Migr~tion  Ev~lu~tor to e~ch VM.  Review the collected d~t~ in ;;m~zon QuickSight. Identify servers th~t h~ve high utiliz~tion.  Remove the servers th~t h~ve high utiliz~tion from the migr~tion list.  Import the d~t~ to ;;WS Migr~tion  Hub.
  B.  Export the VMw~re portfolio to ~ .csv  le. Check the disk utiliz~tion for e~ch server.  Remove servers th~t h~ve high utiliz~tion.  Export the d~t~ to ;;WS ;;pplic~tion  Migr~tion Service. Use ;;WS Server  Migr~tion Service (;;WS SMS) to migr~te the rem~ining servers.
  C.  Deploy the  Migr~tion  Ev~lu~tor ~gentless collector to the  ESXi hypervisor.  Review the collected d~t~ in  Migr~tion  Ev~lu~tor.  Identify in~ctive servers.  Remove the in~ctive servers from the migr~tion list.  Import the d~t~ to ;;WS  Migr~tion  Hub.
  D.  Deploy the ;;WS ;;pplic~tion  Migr~tion Service ;;gent to e~ch VM. When the d~t~ is collected, use ;;m~zon  Redshift to import ~nd ~n~lyze the d~t~. Use ;;m~zon QuickSight for d~t~ visu~liz~tion.

 Correct ;;nswer: C
 C (100%)

 Question #212
 ;; comp~ny runs ~ microservice ~s ~n ;;WS  L~mbd~ function. The microservice writes d~t~ to ~n on-premises SQL d~t~b~se th~t supports ~ limited number of concurrent connections. When the number of  L~mbd~ function invoc~tions is too high, the d~t~b~se cr~shes ~nd c~uses ~pplic~tion downtime. The comp~ny h~s ~n ;;WS  Direct Connect connection between the comp~ny's VPC ~nd the on-premises d~t~ center. The comp~ny w~nts to protect the d~t~b~se from cr~shes. Which solution will meet these requirements?
  ;;. Write the d~t~ to ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Con gure the  L~mbd~ function to re~d from the queue ~nd write to the existing d~t~b~se. Set ~ reserved concurrency limit on the  L~mbd~ function th~t is less th~n the number of connections th~t the d~t~b~se supports.
  B. Cre~te ~ new ;;m~zon ;;uror~ Serverless  DB cluster. Use ;;WS  D~t~Sync to migr~te the d~t~ from the existing d~t~b~se to ;;uror~ Serverless. Recon gure the  L~mbd~ function to write to ;;uror~.
  C. Cre~te ~n ;;m~zon  RDS  Proxy  DB inst~nce. ;;tt~ch the  RDS  Proxy  DB inst~nce to the ;;m~zon  RDS  DB inst~nce.  Recon gure the  L~mbd~ function to write to the  RDS  Proxy  DB inst~nce.
  D. Write the d~t~ to ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic.  Invoke the  L~mbd~ function to write to the existing d~t~b~se when the topic receives new mess~ges. Con gure provisioned concurrency for the  L~mbd~ function to be equ~l to the number of connections th~t the d~t~b~se supports.

 Correct ;;nswer: D
 ;; (95%)                                    5%

 Question #213
 ;; comp~ny uses ~ Gr~f~n~ d~t~ visu~liz~tion solution th~t runs on ~ single ;;m~zon  EC2 inst~nce to monitor the he~lth of the comp~ny's ;;WS worklo~ds. The comp~ny h~s invested time ~nd effort to cre~te d~shbo~rds th~t the comp~ny w~nts to preserve. The d~shbo~rds need to be highly ~v~il~ble ~nd c~nnot be down for longer th~n  10 minutes. The comp~ny needs to minimize ongoing m~inten~nce. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;.  Migr~te to ;;m~zon CloudW~tch d~shbo~rds.  Recre~te the d~shbo~rds to m~tch the existing Gr~f~n~ d~shbo~rds. Use ~utom~tic d~shbo~rds where possible.
  B. Cre~te ~n ;;m~zon  M~n~ged Gr~f~n~ worksp~ce. Con gure ~ new ;;m~zon CloudW~tch d~t~ source.  Export d~shbo~rds from the existing Gr~f~n~ inst~nce.  Import the d~shbo~rds into the new worksp~ce.
  C. Cre~te ~n ;;MI th~t h~s Gr~f~n~ pre-inst~lled. Store the existing d~shbo~rds in ;;m~zon  El~stic  File System (;;m~zon  EFS). Cre~te ~n ;;uto Sc~ling group th~t uses the new ;;MI. Set the ;;uto Sc~ling group's minimum, desired, ~nd m~ximum number of inst~nces to one. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer th~t serves ~t le~st two ;;v~il~bility Zones.
  D. Con gure ;;WS  B~ckup to b~ck up the  EC2 inst~nce th~t runs Gr~f~n~ once e~ch hour.  Restore the  EC2 inst~nce from the most recent sn~pshot in ~n ~ltern~te ;;v~il~bility Zone when required.

 Correct ;;nswer: B
 B (100%)

 Question #214
 ;; comp~ny needs to migr~te its customer tr~ns~ctions d~t~b~se from on premises to ;;WS. The d~t~b~se resides on ~n Or~cle  DB inst~nce th~t runs on ~  Linux server. ;;ccording to ~ new security requirement, the comp~ny must rot~te the d~t~b~se p~ssword e~ch ye~r. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Convert the d~t~b~se to ;;m~zon  Dyn~moDB by using the ;;WS Schem~ Conversion Tool (;;WS SCT). Store the p~ssword in ;;WS Systems M~n~ger  P~r~meter Store. Cre~te ~n ;;m~zon CloudW~tch ~l~rm to invoke ~n ;;WS  L~mbd~ function for ye~rly p~sst~rd rot~tion.
  B.  Migr~te the d~t~b~se to ;;m~zon  RDS for Or~cle. Store the p~ssword in ;;WS Secrets  M~n~ger. Turn on ~utom~tic rot~tion. Con gure ~ ye~rly rot~tion schedule.
  C.  Migr~te the d~t~b~se to ~n ;;m~zon  EC2 inst~nce. Use ;;WS Systems  M~n~ger  P~r~meter Store to keep ~nd rot~te the connection string by using ~n ;;WS  L~mbd~ function on ~ ye~rly schedule.
  D.  Migr~te the d~t~b~se to ;;m~zon  Neptune by using the ;;WS Schem~ Conversion Tool (;;WS SCT). Cre~te ~n ;;m~zon CloudW~tch ~l~rm to invoke ~n ;;WS  L~mbd~ function for ye~rly p~ssword rot~tion.

 Correct ;;nswer: C
 B (100%)

 Question #215
 ;; solutions ~rchitect is designing ~n ;;WS ~ccount structure for ~ comp~ny th~t consists of multiple te~ms. ;;ll the te~ms will work in the s~me ;;WS  Region. The comp~ny needs ~ VPC th~t is connected to the on-premises network. The comp~ny expects less th~n 50  Mbps of tot~l tr~ c to ~nd from the on-premises network. Which combin~tion of steps will meet these requirements  MOST cost-effectively? (Choose two.)
  ;;. Cre~te ~n ;;WS CloudForm~tion templ~te th~t provisions ~ VPC ~nd the required subnets.  Deploy the templ~te to e~ch ;;WS ~ccount.
  B. Cre~te ~n ;;WS CloudForm~tion templ~te th~t provisions ~ VPC ~nd the required subnets.  Deploy the templ~te to ~ sh~red services ~ccount. Sh~re the subnets by using ;;WS  Resource ;;ccess  M~n~ger.
  C. Use ;;WS Tr~nsit G~tew~y ~long with ~n ;;WS Site-to-Site VPN for connectivity to the on-premises network. Sh~re the tr~nsit g~tew~y by using ;;WS  Resource ;;ccess  M~n~ger.
  D. Use ;;WS Site-to-Site VPN for connectivity to the on-premises network.
  E. Use ;;WS  Direct Connect for connectivity to the on-premises network.

 Correct ;;nswer: ;;D
 BD (68%)                             BC (21%)       11%

 Question #216
 ;; solutions ~rchitect ~t ~ l~rge comp~ny needs to set up network security for outbound tr~ c to the internet from ~ll ;;WS ~ccounts within ~n org~niz~tion in ;;WS Org~niz~tions. The org~niz~tion h~s more th~n  100 ;;WS ~ccounts, ~nd the ~ccounts route to e~ch other by using ~ centr~lized ;;WS Tr~nsit G~tew~y.  E~ch ~ccount h~s both ~n internet g~tew~y ~nd ~  N;;T g~tew~y for outbound tr~ c to the internet. The comp~ny deploys resources only into ~ single ;;WS  Region. The comp~ny needs the ~bility to ~dd centr~lly m~n~ged rule-b~sed  ltering on ~ll outbound tr~ c to the internet for ~ll ;;WS ~ccounts in the org~niz~tion. The pe~k lo~d of outbound tr~ c will not exceed 25 Gbps in e~ch ;;v~il~bility Zone. Which solution meets these requirements?
  ;;. Cre~te ~ new VPC for outbound tr~ c to the internet. Connect the existing tr~nsit g~tew~y to the new VPC. Con gure ~ new  N;;T g~tew~y. Cre~te ~n ;;uto Sc~ling group of ;;m~zon  EC2 inst~nces th~t run ~n open-source internet proxy for rule-b~sed  ltering ~cross ~ll ;;v~il~bility Zones in the  Region.  Modify ~ll def~ult routes to point to the proxy's ;;uto Sc~ling group.
  B. Cre~te ~ new VPC for outbound tr~ c to the internet. Connect the existing tr~nsit g~tew~y to the new VPC. Con gure ~ new  N;;T g~tew~y. Use ~n ;;WS  Network  Firew~ll  rew~ll for rule-b~sed  ltering. Cre~te  Network  Firew~ll endpoints in e~ch ;;v~il~bility Zone.  Modify ~ll def~ult routes to point to the  Network  Firew~ll endpoints.
  C. Cre~te ~n ;;WS  Network  Firew~ll  rew~ll for rule-b~sed  ltering in e~ch ;;WS ~ccount.  Modify ~ll def~ult routes to point to the  Network Firew~ll  rew~lls in e~ch ~ccount.
  D.  In e~ch ;;WS ~ccount, cre~te ~n ;;uto Sc~ling group of network-optimized ;;m~zon  EC2 inst~nces th~t run ~n open-source internet proxy for rule-b~sed  ltering.  Modify ~ll def~ult routes to point to the proxy's ;;uto Sc~ling group.

 Correct ;;nswer: D
 B (100%)

 Question #217
 ;; comp~ny uses ~ lo~d b~l~ncer to distribute tr~ c to ;;m~zon  EC2 inst~nces in ~ single ;;v~il~bility Zone. The comp~ny is concerned ~bout security ~nd w~nts ~ solutions ~rchitect to re-~rchitect the solution to meet the following requirements: •  Inbound requests must be  ltered for common vulner~bility ~tt~cks. •  Rejected requests must be sent to ~ third-p~rty ~uditing ~pplic~tion. • ;;ll resources should be highly ~v~il~ble. Which solution meets these requirements?
  ;;. Con gure ~  Multi-;;Z ;;uto Sc~ling group using the ~pplic~tion's ;;MI. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd select the previously cre~ted ;;uto Sc~ling group ~s the t~rget. Use ;;m~zon  Inspector to monitor tr~ c to the ;;LB ~nd  EC2 inst~nces. Cre~te ~ web ;;CL in W;;F. Cre~te ~n ;;WS W;;F using the web ;;CL ~nd ;;LB. Use ~n ;;WS  L~mbd~ function to frequently push the ;;m~zon  Inspector report to the third- p~rty ~uditing ~pplic~tion.
  B. Con gure ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd ~dd the  EC2 inst~nces ~s t~rgets. Cre~te ~ web ;;CL in W;;F. Cre~te ~n ;;WS W;;F using the web ;;CL ~nd ;;LB n~me ~nd en~ble logging with ;;m~zon CloudW~tch  Logs. Use ~n ;;WS  L~mbd~ function to frequently push the logs to the third-p~rty ~uditing ~pplic~tion.
  C. Con gure ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~long with ~ t~rget group ~dding the  EC2 inst~nces ~s t~rgets. Cre~te ~n ;;m~zon  Kinesis D~t~  Firehose with the destin~tion of the third-p~rty ~uditing ~pplic~tion. Cre~te ~ web ;;CL in W;;F. Cre~te ~n ;;WS W;;F using the web ;;CL ~nd ;;LB then en~ble logging by selecting the  Kinesis  D~t~  Firehose ~s the destin~tion. Subscribe to ;;WS  M~n~ged  Rules in ;;WS  M~rketpl~ce, choosing the W;;F ~s the subscriber.
  D. Con gure ~  Multi-;;Z ;;uto Sc~ling group using the ~pplic~tion's ;;MI. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd select the previously cre~ted ;;uto Sc~ling group ~s the t~rget. Cre~te ~n ;;m~zon  Kinesis  D~t~  Firehose with ~ destin~tion of the third-p~rty ~uditing ~pplic~tion. Cre~te ~ web ;;CL in W;;F. Cre~te ~n ;;WS W;;F using the Web;;CL ~nd ;;LB then en~ble logging by selecting the  Kinesis  D~t~  Firehose ~s the destin~tion. Subscribe to ;;WS  M~n~ged  Rules in ;;WS  M~rketpl~ce, choosing the W;;F ~s the subscriber.

 Correct ;;nswer: B
 D (78%)                                ;; (17%)    4%

 Question #218
 ;; comp~ny is running ~n ~pplic~tion in the ;;WS Cloud. The ~pplic~tion consists of microservices th~t run on ~  eet of ;;m~zon  EC2 inst~nces in multiple ;;v~il~bility Zones behind ~n ;;pplic~tion  Lo~d  B~l~ncer. The comp~ny recently ~dded ~ new  REST ;;PI th~t w~s implemented in ;;m~zon ;;PI G~tew~y. Some of the older microservices th~t run on  EC2 inst~nces need to c~ll this new ;;PI. The comp~ny does not w~nt the ;;PI to be ~ccessible from the public internet ~nd does not w~nt propriet~ry d~t~ to tr~verse the public internet. Wh~t should ~ solutions ~rchitect do to meet these requirements?
  ;;. Cre~te ~n ;;WS Site-to-Site VPN connection between the VPC ~nd the ;;PI G~tew~y. Use ;;PI G~tew~y to gener~te ~ unique ;;PI  Key for e~ch microservice. Con gure the ;;PI methods to require the key.
  B. Cre~te ~n interf~ce VPC endpoint for ;;PI G~tew~y, ~nd set ~n endpoint policy to only ~llow ~ccess to the speci c ;;PI. ;;dd ~ resource policy to ;;PI G~tew~y to only ~llow ~ccess from the VPC endpoint. Ch~nge the ;;PI G~tew~y endpoint type to priv~te.
  C.  Modify the ;;PI G~tew~y to use  I;;M ~uthentic~tion. Upd~te the  I;;M policy for the  I;;M role th~t is ~ssigned to the  EC2 inst~nces to ~llow ~ccess to the ;;PI G~tew~y.  Move the ;;PI G~tew~y into ~ new VPDeploy ~ tr~nsit g~tew~y ~nd connect the VPCs.
  D. Cre~te ~n ~cceler~tor in ;;WS Glob~l ;;cceler~tor, ~nd connect the ~cceler~tor to the ;;PI G~tew~y. Upd~te the route t~ble for ~ll VPC subnets with ~ route to the cre~ted Glob~l ;;cceler~tor endpoint  IP ~ddress. ;;dd ~n ;;PI key for e~ch service to use for ~uthentic~tion.

 Correct ;;nswer: C
 B (100%)

 Question #219
 ;; comp~ny h~s set up its entire infr~structure on ;;WS. The comp~ny uses ;;m~zon  EC2 inst~nces to host its ecommerce website ~nd uses ;;m~zon S3 to store st~tic d~t~. Three engineers ~t the comp~ny h~ndle the cloud ~dministr~tion ~nd development through one ;;WS ~ccount. Occ~sion~lly, ~n engineer ~lters ~n  EC2 security group con gur~tion of ~nother engineer ~nd c~uses noncompli~nce issues in the environment. ;; solutions ~rchitect must set up ~ system th~t tr~cks ch~nges th~t the engineers m~ke. The system must send ~lerts when the engineers m~ke noncompli~nt ch~nges to the security settings for the  EC2 inst~nces. Wh~t is the  F;;STEST w~y for the solutions ~rchitect to meet these requirements?
  ;;. Set up ;;WS Org~niz~tions for the comp~ny. ;;pply SCPs to govern ~nd tr~ck noncompli~nt security group ch~nges th~t ~re m~de to the ;;WS ~ccount.
  B.  En~ble ;;WS CloudTr~il to c~pture the ch~nges to  EC2 security groups.  En~ble ;;m~zon CloudW~tch rules to provide ~lerts when noncompli~nt security settings ~re detected.
  C.  En~ble SCPs on the ;;WS ~ccount to provide ~lerts when noncompli~nt security group ch~nges ~re m~de to the environment.
  D.  En~ble ;;WS Con g on the  EC2 security groups to tr~ck ~ny noncompli~nt ch~nges. Send the ch~nges ~s ~lerts through ~n ;;m~zon Simple Noti c~tion Service (;;m~zon SNS) topic.

 Correct ;;nswer: B
 D (88%)                                   12%

 Question #220
 ;; comp~ny h~s  IoT sensors th~t monitor tr~ c p~tterns throughout ~ l~rge city. The comp~ny w~nts to re~d ~nd collect d~t~ from the sensors ~nd perform ~ggreg~tions on the d~t~. ;; solutions ~rchitect designs ~ solution in which the  IoT devices ~re stre~ming to ;;m~zon  Kinesis  D~t~ Stre~ms. Sever~l ~pplic~tions ~re re~ding from the stre~m.  However, sever~l consumers ~re experiencing throttling ~nd ~re periodic~lly encountering ~ Re~dProvisionedThroughputExceeded error. Which ~ctions should the solutions ~rchitect t~ke to resolve this issue? (Choose three.)
  ;;.  Resh~rd the stre~m to incre~se the number of sh~rds in the stre~m.
  B. Use the  Kinesis  Producer  Libr~ry (KPL). ;;djust the polling frequency.
  C. Use consumers with the enh~nced f~n-out fe~ture.
  D.  Resh~rd the stre~m to reduce the number of sh~rds in the stre~m.
  E. Use ~n error retry ~nd exponenti~l b~ckoff mech~nism in the consumer logic.
  F. Con gure the stre~m to use dyn~mic p~rtitioning.

 Correct ;;nswer: ;;CE
 ;;CE (100%)

 Question #221
 ;; comp~ny uses ;;WS Org~niz~tions to m~n~ge its ;;WS ~ccounts. The comp~ny needs ~ list of ~ll its ;;m~zon  EC2 inst~nces th~t h~ve underutilized CPU or memory us~ge. The comp~ny ~lso needs recommend~tions for how to downsize these underutilized inst~nces. Which solution will meet these requirements with the  LE;;ST effort?
  ;;.  Inst~ll ~ CPU ~nd memory monitoring tool from ;;WS  M~rketpl~ce on ~ll the  EC2 inst~nces. Store the  ndings in ;;m~zon S3.  Implement ~ Python script to identify underutilized inst~nces.  Reference  EC2 inst~nce pricing inform~tion for recommend~tions ~bout downsizing options.
  B.  Inst~ll the ;;m~zon CloudW~tch ~gent on ~ll the  EC2 inst~nces by using ;;WS Systems  M~n~ger.  Retrieve the resource optimiz~tion recommend~tions from ;;WS Cost  Explorer in the org~niz~tion’s m~n~gement ~ccount. Use the recommend~tions to downsize underutilized inst~nces in ~ll ~ccounts of the org~niz~tion.
  C.  Inst~ll the ;;m~zon CloudW~tch ~gent on ~ll the  EC2 inst~nces by using ;;WS Systems  M~n~ger.  Retrieve the resource optimiz~tion recommend~tions from ;;WS Cost  Explorer in e~ch ~ccount of the org~niz~tion. Use the recommend~tions to downsize underutilized inst~nces in ~ll ~ccounts of the org~niz~tion.
  D.  Inst~ll the ;;m~zon CloudW~tch ~gent on ~ll the  EC2 inst~nces by using ;;WS Systems  M~n~ger. Cre~te ~n ;;WS  L~mbd~ function to extr~ct CPU ~nd memory us~ge from ~ll the  EC2 inst~nces. Store the  ndings ~s  les in ;;m~zon S3. Use ;;m~zon ;;then~ to  nd underutilized inst~nces.  Reference  EC2 inst~nce pricing inform~tion for recommend~tions ~bout downsizing options.

 Correct ;;nswer: B
 B (100%)

 Question #222
 ;; comp~ny w~nts to run ~ custom network ~n~lysis softw~re p~ck~ge to inspect tr~ c ~s tr~ c le~ves ~nd enters ~ VPC. The comp~ny h~s deployed the solution by using ;;WS CloudForm~tion on three ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group. ;;ll network routing h~s been est~blished to direct tr~ c to the  EC2 inst~nces. Whenever the ~n~lysis softw~re stops working, the ;;uto Sc~ling group repl~ces ~n inst~nce. The network routes ~re not upd~ted when the inst~nce repl~cement occurs. Which combin~tion of steps will resolve this issue? (Choose three.)
  ;;. Cre~te ~l~rms b~sed on  EC2 st~tus check metrics th~t will c~use the ;;uto Sc~ling group to repl~ce the f~iled inst~nce.
  B. Upd~te the CloudForm~tion templ~te to inst~ll the ;;m~zon CloudW~tch ~gent on the  EC2 inst~nces. Con gure the CloudW~tch ~gent to send process metrics for the ~pplic~tion.
  C. Upd~te the CloudForm~tion templ~te to inst~ll ;;WS Systems  M~n~ger ;;gent on the  EC2 inst~nces. Con gure Systems  M~n~ger ;;gent to send process metrics for the ~pplic~tion.
  D. Cre~te ~n ~l~rm for the custom metric in ;;m~zon CloudW~tch for the f~ilure scen~rios. Con gure the ~l~rm to publish ~ mess~ge to ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic.
  E. Cre~te ~n ;;WS  L~mbd~ function th~t responds to the ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) mess~ge to t~ke the inst~nce out of service. Upd~te the network routes to point to the repl~cement inst~nce.
  F.  In the CloudForm~tion templ~te, write ~ condition th~t upd~tes the network routes when ~ repl~cement inst~nce is l~unched.

 Correct ;;nswer: ;;DF
 BDE (100%)

 Question #223
 ;; comp~ny is developing ~ new on-dem~nd video ~pplic~tion th~t is b~sed on microservices. The ~pplic~tion will h~ve 5 million users ~t l~unch ~nd will h~ve 30 million users ~fter 6 months. The comp~ny h~s deployed the ~pplic~tion on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ;;WS  F~rg~te. The comp~ny developed the ~pplic~tion by using  ECS services th~t use the  HTTPS protocol. ;; solutions ~rchitect needs to implement upd~tes to the ~pplic~tion by using blue/green deployments. The solution must distribute tr~ c to e~ch ECS service through ~ lo~d b~l~ncer. The ~pplic~tion must ~utom~tic~lly ~djust the number of t~sks in response to ~n ;;m~zon CloudW~tch ~l~rm. Which solution will meet these requirements?
  ;;. Con gure the  ECS services to use the blue/green deployment type ~nd ~  Network  Lo~d  B~l~ncer.  Request incre~ses to the service quot~ for t~sks per service to meet the dem~nd.
  B. Con gure the  ECS services to use the blue/green deployment type ~nd ~  Network  Lo~d  B~l~ncer.  Implement ;;uto Sc~ling group for e~ch ECS service by using the Cluster ;;utosc~ler.
  C. Con gure the  ECS services to use the blue/green deployment type ~nd ~n ;;pplic~tion  Lo~d  B~l~ncer.  Implement ~n ;;uto Sc~ling group for e~ch  ECS service by using the Cluster ;;utosc~ler.
  D. Con gure the  ECS services to use the blue/green deployment type ~nd ~n ;;pplic~tion  Lo~d  B~l~ncer.  Implement Service ;;uto Sc~ling for e~ch  ECS service.

 Correct ;;nswer: ;;
 D (88%)                                    13%

 Question #224
 ;; comp~ny is running ~ cont~inerized ~pplic~tion in the ;;WS Cloud. The ~pplic~tion is running by using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ~ set of ;;m~zon  EC2 inst~nces. The  EC2 inst~nces run in ~n ;;uto Sc~ling group. The comp~ny uses ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR) to store its cont~iner im~ges. When ~ new im~ge version is uplo~ded, the new im~ge version receives ~ unique t~g. The comp~ny needs ~ solution th~t inspects new im~ge versions for common vulner~bilities ~nd exposures. The solution must ~utom~tic~lly delete new im~ge t~gs th~t h~ve Critic~l or  High severity  ndings. The solution ~lso must notify the development te~m when such ~ deletion occurs. Which solution meets these requirements?
  ;;. Con gure sc~n on push on the repository. Use ;;m~zon  EventBridge to invoke ~n ;;WS Step  Functions st~te m~chine when ~ sc~n is complete for im~ges th~t h~ve Critic~l or  High severity  ndings. Use the Step  Functions st~te m~chine to delete the im~ge t~g for those im~ges ~nd to notify the development te~m through ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS).
  B. Con gure sc~n on push on the repository. Con gure sc~n results to be pushed to ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Invoke ~n ;;WS  L~mbd~ function when ~ new mess~ge is ~dded to the SQS queue. Use the  L~mbd~ function to delete the im~ge t~g for im~ges th~t h~ve Critic~l or  High severity  ndings.  Notify the development te~m by using ;;m~zon Simple  Em~il Service (;;m~zon SES).
  C. Schedule ~n ;;WS  L~mbd~ function to st~rt ~ m~nu~l im~ge sc~n every hour. Con gure ;;m~zon  EventBridge to invoke ~nother  L~mbd~ function when ~ sc~n is complete. Use the second  L~mbd~ function to delete the im~ge t~g for im~ges th~t h~ve Critic~l or  High severity  ndings.  Notify the development te~m by using ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS).
  D. Con gure periodic im~ge sc~n on the repository. Con gure sc~n results to be ~dded to ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue.  Invoke ~n ;;WS Step  Functions st~te m~chine when ~ new mess~ge is ~dded to the SQS queue. Use the Step  Functions st~te m~chine to delete the im~ge t~g for im~ges th~t h~ve Critic~l or  High severity  ndings.  Notify the development te~m by using ;;m~zon Simple  Em~il Service (;;m~zon SES).

 Correct ;;nswer: C
 ;; (100%)

 Question #225
 ;; comp~ny runs m~ny worklo~ds on ;;WS ~nd uses ;;WS Org~niz~tions to m~n~ge its ~ccounts. The worklo~ds ~re hosted on ;;m~zon  EC2. ;;WS F~rg~te. ~nd ;;WS  L~mbd~. Some of the worklo~ds h~ve unpredict~ble dem~nd. ;;ccounts record high us~ge in some months ~nd low us~ge in other months. The comp~ny w~nts to optimize its compute costs over the next 3 ye~rs. ;; solutions ~rchitect obt~ins ~ 6-month ~ver~ge for e~ch of the ~ccounts ~cross the org~niz~tion to c~lcul~te us~ge. Which solution will provide the  MOST cost s~vings for ~ll the org~niz~tion's compute us~ge?
  ;;.  Purch~se  Reserved  Inst~nces for the org~niz~tion to m~tch the size ~nd number of the most common  EC2 inst~nces from the member ~ccounts.
  B.  Purch~se ~ Compute S~vings  Pl~n for the org~niz~tion from the m~n~gement ~ccount by using the recommend~tion ~t the m~n~gement ~ccount level.
  C.  Purch~se  Reserved  Inst~nces for e~ch member ~ccount th~t h~d high  EC2 us~ge ~ccording to the d~t~ from the l~st 6 months.
  D.  Purch~se ~n  EC2  Inst~nce S~vings  Pl~n for e~ch member ~ccount from the m~n~gement ~ccount b~sed on  EC2 us~ge d~t~ from the l~st 6 months.

 Correct ;;nswer: B
 B (100%)

 Question #226
 ;; comp~ny h~s hundreds of ;;WS ~ccounts. The comp~ny uses ~n org~niz~tion in ;;WS Org~niz~tions to m~n~ge ~ll the ~ccounts. The comp~ny h~s turned on ~ll fe~tures. ;;  n~nce te~m h~s ~lloc~ted ~ d~ily budget for ;;WS costs. The  n~nce te~m must receive ~n em~il noti c~tion if the org~niz~tion's ;;WS costs exceed 80% of the ~lloc~ted budget. ;; solutions ~rchitect needs to implement ~ solution to tr~ck the costs ~nd deliver the noti c~tions. Which solution will meet these requirements?
  ;;.  In the org~niz~tion's m~n~gement ~ccount, use ;;WS  Budgets to cre~te ~ budget th~t h~s ~ d~ily period. ;;dd ~n ~lert threshold ~nd set the v~lue to 80%. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to notify the  n~nce te~m.
  B.  In the org~niz~tion’s m~n~gement ~ccount, set up the org~niz~tion~l view fe~ture for ;;WS Trusted ;;dvisor. Cre~te ~n org~niz~tion~l view report for cost optimiz~tion. Set ~n ~lert threshold of 80%. Con gure noti c~tion preferences. ;;dd the em~il ~ddresses of the  n~nce te~m.
  C.  Register the org~niz~tion with ;;WS Control Tower. ;;ctiv~te the option~l cost control (gu~rdr~il). Set ~ control (gu~rdr~il) p~r~meter of 80%. Con gure control (gu~rdr~il) noti c~tion preferences. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to notify the  n~nce te~m.
  D. Con gure the member ~ccounts to s~ve ~ d~ily ;;WS Cost ~nd Us~ge  Report to ~n ;;m~zon S3 bucket in the org~niz~tion's m~n~gement ~ccount. Use ;;m~zon  EventBridge to schedule ~ d~ily ;;m~zon ;;then~ query to c~lcul~te the org~niz~tion’s costs. Con gure ;;then~ to send ~n ;;m~zon CloudW~tch ~lert if the tot~l costs ~re more th~n 80% of the ~lloc~ted budget. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to notify the  n~nce te~m.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #227
 ;; comp~ny provides ~uction services for ~rtwork ~nd h~s users ~cross  North ;;meric~ ~nd  Europe. The comp~ny hosts its ~pplic~tion in ;;m~zon EC2 inst~nces in the us-e~st-1  Region. ;;rtists uplo~d photos of their work ~s l~rge-size. high-resolution im~ge  les from their mobile phones to ~ centr~lized ;;m~zon S3 bucket cre~ted in the us-e~st-1  Region. The users in  Europe ~re reporting slow perform~nce for their im~ge uplo~ds. How c~n ~ solutions ~rchitect improve the perform~nce of the im~ge uplo~d process?
  ;;.  Redeploy the ~pplic~tion to use S3 multip~rt uplo~ds.
  B. Cre~te ~n ;;m~zon CloudFront distribution ~nd point to the ~pplic~tion ~s ~ custom origin.
  C. Con gure the buckets to use S3 Tr~nsfer ;;cceler~tion.
  D. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces ~nd cre~te ~ sc~ling policy.

 Correct ;;nswer: C
 C (89%)                                    11%

 Question #228
 ;; comp~ny w~nts to cont~inerize ~ multi-tier web ~pplic~tion ~nd move the ~pplic~tion from ~n on-premises d~t~ center to ;;WS. The ~pplic~tion includes web. ~pplic~tion, ~nd d~t~b~se tiers. The comp~ny needs to m~ke the ~pplic~tion f~ult toler~nt ~nd sc~l~ble. Some frequently ~ccessed d~t~ must ~lw~ys be ~v~il~ble ~cross ~pplic~tion servers.  Frontend web servers need session persistence ~nd must sc~le to meet incre~ses in tr~ c. Which solution will meet these requirements with the  LE;;ST ongoing oper~tion~l overhe~d?
  ;;.  Run the ~pplic~tion on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ;;WS  F~rg~te. Use ;;m~zon  El~stic  File System (;;m~zon  EFS) for d~t~ th~t is frequently ~ccessed between the web ~nd ~pplic~tion tiers. Store the frontend web server session d~t~ in ;;m~zon Simple Queue Service (;;m~zon SQS).
  B.  Run the ~pplic~tion on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ;;m~zon  EC2. Use ;;m~zon  El~stiC~che for  Redis to c~che frontend web server session d~t~. Use ;;m~zon  El~stic  Block Store (;;m~zon  EBS) with  Multi-;;tt~ch on  EC2 inst~nces th~t ~re distributed ~cross multiple ;;v~il~bility Zones.
  C.  Run the ~pplic~tion on ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS). Con gure ;;m~zon  EKS to use m~n~ged node groups. Use Replic~Sets to run the web servers ~nd ~pplic~tions. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system.  Mount the  EFS  le system ~cross ~ll  EKS pods to store frontend web server session d~t~.
  D.  Deploy the ~pplic~tion on ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS). Con gure ;;m~zon  EKS to use m~n~ged node groups.  Run the web servers ~nd ~pplic~tion ~s  Kubernetes deployments in the  EKS cluster. Store the frontend web server session d~t~ in ~n ;;m~zon Dyn~moDB t~ble. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS) volume th~t ~ll ~pplic~tions will mount ~t the time of deployment.

 Correct ;;nswer: B
 D (85%)                                   Other

 Question #229
 ;; solutions ~rchitect is pl~nning to migr~te critic~l  Microsoft SQL Server d~t~b~ses to ;;WS.  Bec~use the d~t~b~ses ~re leg~cy systems, the solutions ~rchitect will move the d~t~b~ses to ~ modern d~t~ ~rchitecture. The solutions ~rchitect must migr~te the d~t~b~ses with ne~r-zero downtime. Which solution will meet these requirements?
  ;;. Use ;;WS ;;pplic~tion  Migr~tion Service ~nd the ;;WS Schem~ Conversion Tool (;;WS SCT).  Perform ~n in-pl~ce upgr~de before the migr~tion.  Export the migr~ted d~t~ to ;;m~zon ;;uror~ Serverless ~fter cutover.  Repoint the ~pplic~tions to ;;m~zon ;;uror~.
  B. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to rehost the d~t~b~se. Set ;;m~zon S3 ~s ~ t~rget. Set up ch~nge d~t~ c~pture (CDC) replic~tion. When the source ~nd destin~tion ~re fully synchronized, lo~d the d~t~ from ;;m~zon S3 into ~n ;;m~zon  RDS for  Microsoft SQL Server  DB inst~nce.
  C. Use n~tive d~t~b~se high ~v~il~bility tools. Connect the source system to ~n ;;m~zon  RDS for  Microsoft SQL Server  DB inst~nce. Con gure replic~tion ~ccordingly. When d~t~ replic~tion is  nished, tr~nsition the worklo~d to ~n ;;m~zon  RDS for  Microsoft SQL Server  DB inst~nce.
  D. Use ;;WS ;;pplic~tion  Migr~tion Service.  Rehost the d~t~b~se server on ;;m~zon  EC2. When d~t~ replic~tion is  nished, det~ch the d~t~b~se ~nd move the d~t~b~se to ~n ;;m~zon  RDS for  Microsoft SQL Server  DB inst~nce.  Re~tt~ch the d~t~b~se ~nd then cut over ~ll networking.

 Correct ;;nswer: C
 C (63%)                                  B (37%)

 Question #230
 ;; comp~ny's solutions ~rchitect is ~n~lyzing costs of ~ multi-~pplic~tion environment. The environment is deployed ~cross multiple ;;v~il~bility Zones in ~ single ;;WS  Region. ;;fter ~ recent ~cquisition, the comp~ny m~n~ges two org~niz~tions in ;;WS Org~niz~tions. The comp~ny h~s cre~ted multiple service provider ~pplic~tions ~s ;;WS  Priv~teLink-powered VPC endpoint services in one org~niz~tion. The comp~ny h~s cre~ted multiple service consumer ~pplic~tions in the other org~niz~tion. D~t~ tr~nsfer ch~rges ~re much higher th~n the comp~ny expected, ~nd the solutions ~rchitect needs to reduce the costs. The solutions ~rchitect must recommend guidelines for developers to follow when they deploy services. These guidelines must minimize d~t~ tr~nsfer ch~rges for the whole environment. Which guidelines meet these requirements? (Choose two.)
  ;;. Use ;;WS  Resource ;;ccess  M~n~ger to sh~re the subnets th~t host the service provider ~pplic~tions with other ~ccounts in the org~niz~tion.
  B.  Pl~ce the service provider ~pplic~tions ~nd the service consumer ~pplic~tions in ;;WS ~ccounts in the s~me org~niz~tion.
  C. Turn off cross-zone lo~d b~l~ncing for the  Network  Lo~d  B~l~ncer in ~ll service provider ~pplic~tion deployments.
  D.  Ensure th~t service consumer compute resources use the ;;v~il~bility Zone-speci c endpoint service by using the endpoint's loc~l  DNS n~me.
  E. Cre~te ~ S~vings  Pl~n th~t provides ~dequ~te cover~ge for the org~niz~tion's pl~nned inter-;;v~il~bility Zone d~t~ tr~nsfer us~ge.

 Correct ;;nswer: ;;B
 BD (37%)                    CD (32%)               ;;D (26%)       5%

 Question #231
 ;; comp~ny h~s ~n on-premises  Microsoft SQL Server d~t~b~se th~t writes ~ nightly 200 GB export to ~ loc~l drive. The comp~ny w~nts to move the b~ckups to more robust cloud stor~ge on ;;m~zon S3. The comp~ny h~s set up ~  10 Gbps ;;WS  Direct Connect connection between the on- premises d~t~ center ~nd ;;WS. Which solution meets these requirements  MOST cost-effectively?
  ;;. Cre~te ~ new S3 bucket.  Deploy ~n ;;WS Stor~ge G~tew~y  le g~tew~y within the VPC th~t is connected to the  Direct Connect connection. Cre~te ~ new SMB  le sh~re. Write nightly d~t~b~se exports to the new SMB  le sh~re.
  B. Cre~te ~n ;;m~zon  FSx for Windows  File Server Single-;;Z  le system within the VPC th~t is connected to the  Direct Connect connection. Cre~te ~ new SMB  le sh~re. Write nightly d~t~b~se exports to ~n SMB  le sh~re on the ;;m~zon  FSx  le system.  En~ble nightly b~ckups.
  C. Cre~te ~n ;;m~zon  FSx for Windows  File Server  Multi-;;Z  le system within the VPC th~t is connected to the  Direct Connect connection. Cre~te ~ new SMB  le sh~re. Write nightly d~t~b~se exports to ~n SMB  le sh~re on the ;;m~zon  FSx  le system.  En~ble nightly b~ckups.
  D. Cre~te ~ new S3 bucket.  Deploy ~n ;;WS Stor~ge G~tew~y volume g~tew~y within the VPC th~t is connected to the  Direct Connect connection. Cre~te ~ new SMB  le sh~re. Write nightly d~t~b~se exports to the new SMB  le sh~re on the volume g~tew~y, ~nd ~utom~te copies of this d~t~ to ~n S3 bucket.

 Correct ;;nswer: ;;
 ;; (93%)                                   7%

 Question #232
 ;; comp~ny needs to est~blish ~ connection from its on-premises d~t~ center to ;;WS. The comp~ny needs to connect ~ll of its VPCs th~t ~re loc~ted in different ;;WS  Regions with tr~nsitive routing c~p~bilities between VPC networks. The comp~ny ~lso must reduce network outbound tr~ c costs, incre~se b~ndwidth throughput, ~nd provide ~ consistent network experience for end users. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;WS Site-to-Site VPN connection between the on-premises d~t~ center ~nd ~ new centr~l VPC. Cre~te VPC peering connections th~t initi~te from the centr~l VPC to ~ll other VPCs.
  B. Cre~te ~n ;;WS  Direct Connect connection between the on-premises d~t~ center ~nd ;;WS.  Provision ~ tr~nsit VIF, ~nd connect it to ~  Direct Connect g~tew~y. Connect the  Direct Connect g~tew~y to ~ll the other VPCs by using ~ tr~nsit g~tew~y in e~ch  Region.
  C. Cre~te ~n ;;WS Site-to-Site VPN connection between the on-premises d~t~ center ~nd ~ new centr~l VPUse ~ tr~nsit g~tew~y with dyn~mic routing. Connect the tr~nsit g~tew~y to ~ll other VPCs.
  D. Cre~te ~n ;;WS  Direct Connect connection between the on-premises d~t~ center ~nd ;;WS.  Est~blish ~n ;;WS Site-to-Site VPN connection between ~ll VPCs in e~ch  Region. Cre~te VPC peering connections th~t initi~te from the centr~l VPC to ~ll other VPCs.

 Correct ;;nswer: B
 B (100%)

 Question #233
 ;; comp~ny is migr~ting its development ~nd production worklo~ds to ~ new org~niz~tion in ;;WS Org~niz~tions. The comp~ny h~s cre~ted ~ sep~r~te member ~ccount for development ~nd ~ sep~r~te member ~ccount for production. Consolid~ted billing is linked to the m~n~gement ~ccount.  In the m~n~gement ~ccount, ~ solutions ~rchitect needs to cre~te ~n  I;;M user th~t c~n stop or termin~te resources in both member ~ccounts. Which solution will meet this requirement?
  ;;. Cre~te ~n  I;;M user ~nd ~ cross-~ccount role in the m~n~gement ~ccount. Con gure the cross-~ccount role with le~st privilege ~ccess to the member ~ccounts.
  B. Cre~te ~n  I;;M user in e~ch member ~ccount.  In the m~n~gement ~ccount, cre~te ~ cross-~ccount role th~t h~s le~st privilege ~ccess. Gr~nt the  I;;M users ~ccess to the cross-~ccount role by using ~ trust policy.
  C. Cre~te ~n  I;;M user in the m~n~gement ~ccount.  In the member ~ccounts, cre~te ~n  I;;M group th~t h~s le~st privilege ~ccess. ;;dd the  I;;M user from the m~n~gement ~ccount to e~ch  I;;M group in the member ~ccounts.
  D. Cre~te ~n  I;;M user in the m~n~gement ~ccount.  In the member ~ccounts, cre~te cross-~ccount roles th~t h~ve le~st privilege ~ccess. Gr~nt the  I;;M user ~ccess to the roles by using ~ trust policy.

 Correct ;;nswer: D
 D (100%)

 Question #234
 ;; comp~ny w~nts to use ;;WS for dis~ster recovery for ~n on-premises ~pplic~tion. The comp~ny h~s hundreds of Windows-b~sed servers th~t run the ~pplic~tion. ;;ll the servers mount ~ common sh~re. The comp~ny h~s ~n  RTO of  15 minutes ~nd ~n  RPO of 5 minutes. The solution must support n~tive f~ilover ~nd f~llb~ck c~p~bilities. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Cre~te ~n ;;WS Stor~ge G~tew~y  File G~tew~y. Schedule d~ily Windows server b~ckups. S~ve the d~t~ to ;;m~zon S3.  During ~ dis~ster, recover the on-premises servers from the b~ckup.  During t~ilb~ck, run the on-premises servers on ;;m~zon  EC2 inst~nces.
  B. Cre~te ~ set of ;;WS CloudForm~tion templ~tes to cre~te infr~structure.  Replic~te ~ll d~t~ to ;;m~zon  El~stic  File System (;;m~zon  EFS) by using ;;WS  D~t~Sync.  During ~ dis~ster, use ;;WS CodePipeline to deploy the templ~tes to restore the on-premises servers.  F~il b~ck the d~t~ by using  D~t~Sync.
  C. Cre~te ~n ;;WS Cloud  Development  Kit (;;WS CDK) pipeline to st~nd up ~ multi-site ~ctive-~ctive environment on ;;WS.  Replic~te d~t~ into ;;m~zon S3 by using the s3 sync comm~nd.  During ~ dis~ster, sw~p  DNS endpoints to point to ;;WS.  F~il b~ck the d~t~ by using the s3 sync comm~nd.
  D. Use ;;WS  El~stic  Dis~ster  Recovery to replic~te the on-premises servers.  Replic~te d~t~ to ~n ;;m~zon  FSx for Windows  File Server  le system by using ;;WS  D~t~Sync.  Mount the  le system to ;;WS servers.  During ~ dis~ster, f~il over the on-premises servers to ;;WS.  F~il b~ck to new or existing servers by using  El~stic  Dis~ster  Recovery.

 Correct ;;nswer: B
 D (100%)

 Question #235
 ;; comp~ny h~s built ~ high perform~nce computing (HPC) cluster in ;;WS for ~ tightly coupled worklo~d th~t gener~tes ~ l~rge number of sh~red  les stored in ;;m~zon  EFS. The cluster w~s performing well when the number of ;;m~zon  EC2 inst~nces in the cluster w~s  100.  However, when the comp~ny incre~sed the cluster size to  1.000  EC2 inst~nces, over~ll perform~nce w~s well below expect~tions. Which collection of design choices should ~ solutions ~rchitect m~ke to ~chieve the m~ximum perform~nce from the  HPC cluster? (Choose three.)
  ;;.  Ensure the  HPC cluster is l~unched within ~ single ;;v~il~bility Zone.
  B.  L~unch the  EC2 inst~nces ~nd ~tt~ch el~stic network interf~ces in multiples of four.
  C. Select  EC2 inst~nce types with ~n  El~stic  F~bric ;;d~pter (EF;;) en~bled.
  D.  Ensure the cluster is l~unched ~cross multiple ;;v~il~bility Zones.
  E.  Repl~ce ;;m~zon  EFS with multiple ;;m~zon  EBS volumes in ~  R;;ID ~rr~y.
  F.  Repl~ce ;;m~zon  EFS with ;;m~zon  FSx for  Lustre.

 Correct ;;nswer: ;;CF
 ;;CF (88%)                                   13%

 Question #236
 ;; comp~ny is designing ~n ;;WS Org~niz~tions structure. The comp~ny w~nts to st~nd~rdize ~ process to ~pply t~gs ~cross the entire org~niz~tion. The comp~ny will require t~gs with speci c v~lues when ~ user cre~tes ~ new resource.  E~ch of the comp~ny's OUs will h~ve unique t~g v~lues. Which solution will meet these requirements?
  ;;. Use ~n SCP to deny the cre~tion of resources th~t do not h~ve the required t~gs. Cre~te ~ t~g policy th~t includes the t~g v~lues th~t the comp~ny h~s ~ssigned to e~ch OU. ;;tt~ch the t~g policies to the OUs.
  B. Use ~n SCP to deny the cre~tion of resources th~t do not h~ve the required t~gs. Cre~te ~ t~g policy th~t includes the t~g v~lues th~t the comp~ny h~s ~ssigned to e~ch OU. ;;tt~ch the t~g policies to the org~niz~tion's m~n~gement ~ccount.
  C. Use ~n SCP to ~llow the cre~tion of resources only when the resources h~ve the required t~gs. Cre~te ~ t~g policy th~t includes the t~g v~lues th~t the comp~ny h~s ~ssigned to e~ch OU. ;;tt~ch the t~g policies to the OUs.
  D. Use ~n SCP to deny the cre~tion of resources th~t do not h~ve the required t~gs.  De ne the list of t~gs. ;;tt~ch the SCP to the OUs.

 Correct ;;nswer: C
 ;; (82%)                                 B (18%)

 Question #237
 ;; comp~ny h~s more th~n  10,000 sensors th~t send d~t~ to ~n on-premises ;;p~che  K~fk~ server by using the  Mess~ge Queuing Telemetry Tr~nsport (MQTT) protocol. The on-premises  K~fk~ server tr~nsforms the d~t~ ~nd then stores the results ~s objects in ~n ;;m~zon S3 bucket. Recently, the  K~fk~ server cr~shed. The comp~ny lost sensor d~t~ while the server w~s being restored. ;; solutions ~rchitect must cre~te ~ new design on ;;WS th~t is highly ~v~il~ble ~nd sc~l~ble to prevent ~ simil~r occurrence. Which solution will meet these requirements?
  ;;.  L~unch two ;;m~zon  EC2 inst~nces to host the  K~fk~ server in ~n ~ctive/st~ndby con gur~tion ~cross two ;;v~il~bility Zones. Cre~te ~ dom~in n~me in ;;m~zon  Route 53. Cre~te ~  Route 53 f~ilover policy.  Route the sensors to send the d~t~ to the dom~in n~me.
  B.  Migr~te the on-premises  K~fk~ server to ;;m~zon  M~n~ged Stre~ming for ;;p~che  K~fk~ (;;m~zon  MSK). Cre~te ~  Network  Lo~d  B~l~ncer (NLB) th~t points to the ;;m~zon  MSK broker.  En~ble  NLB he~lth checks.  Route the sensors to send the d~t~ to the  NLB.
  C.  Deploy ;;WS  IoT Core, ~nd connect it to ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m. Use ~n ;;WS  L~mbd~ function to h~ndle d~t~ tr~nsform~tion.  Route the sensors to send the d~t~ to ;;WS  IoT Core.
  D.  Deploy ;;WS  IoT Core, ~nd l~unch ~n ;;m~zon  EC2 inst~nce to host the  K~fk~ server. Con gure ;;WS  IoT Core to send the d~t~ to the  EC2 inst~nce.  Route the sensors to send the d~t~ to ;;WS  IoT Core.

 Correct ;;nswer: ;;
 C (77%)                                 B (23%)

 Question #238
 ;; comp~ny recently st~rted hosting new ~pplic~tion worklo~ds in the ;;WS Cloud. The comp~ny is using ;;m~zon  EC2 inst~nces. ;;m~zon  El~stic File System (;;m~zon  EFS)  le systems, ~nd ;;m~zon  RDS  DB inst~nces. To meet regul~tory ~nd business requirements, the comp~ny must m~ke the following ch~nges for d~t~ b~ckups: •  B~ckups must be ret~ined b~sed on custom d~ily, weekly, ~nd monthly requirements. •  B~ckups must be replic~ted to ~t le~st one other ;;WS  Region immedi~tely ~fter c~pture. • The b~ckup solution must provide ~ single source of b~ckup st~tus ~cross the ;;WS environment. • The b~ckup solution must send immedi~te noti c~tions upon f~ilure of ~ny resource b~ckup. Which combin~tion of steps will meet these requirements with the  LE;;ST ~mount of oper~tion~l overhe~d? (Choose three.)
  ;;. Cre~te ~n ;;WS  B~ckup pl~n with ~ b~ckup rule for e~ch of the retention requirements.
  B. Con gure ~n ;;WS  B~ckup pl~n to copy b~ckups to ~nother  Region.
  C. Cre~te ~n ;;WS  L~mbd~ function to replic~te b~ckups to ~nother  Region ~nd send noti c~tion if ~ f~ilure occurs.
  D. ;;dd ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic to the b~ckup pl~n to send ~ noti c~tion for  nished jobs th~t h~ve ~ny st~tus except  B;;CKUP_JOB_COMPLETED.
  E. Cre~te ~n ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM) sn~pshot lifecycle policy for e~ch of the retention requirements.
  F. Set up  RDS sn~pshots on e~ch d~t~b~se.

 Correct ;;nswer: ;;BD
 ;;BD (100%)

 Question #239
 ;; comp~ny is developing ~ gene reporting device th~t will collect genomic inform~tion to ~ssist rese~rchers with collecting l~rge s~mples of d~t~ from ~ diverse popul~tion. The device will push 8  KB of genomic d~t~ every second to ~ d~t~ pl~tform th~t will need to process ~nd ~n~lyze the d~t~ ~nd provide inform~tion b~ck to rese~rchers. The d~t~ pl~tform must meet the following requirements: •  Provide ne~r-re~l-time ~n~lytics of the inbound genomic d~t~ •  Ensure the d~t~ is  exible, p~r~llel, ~nd dur~ble •  Deliver results of processing to ~ d~t~ w~rehouse Which str~tegy should ~ solutions ~rchitect use to meet these requirements?
  ;;. Use ;;m~zon  Kinesis  D~t~  Firehose to collect the inbound sensor d~t~, ~n~lyze the d~t~ with  Kinesis clients, ~nd s~ve the results to ~n ;;m~zon  RDS inst~nce.
  B. Use ;;m~zon  Kinesis  D~t~ Stre~ms to collect the inbound sensor d~t~, ~n~lyze the d~t~ with  Kinesis clients, ~nd s~ve the results to ~n ;;m~zon  Redshift cluster using ;;m~zon  EMR.
  C. Use ;;m~zon S3 to collect the inbound device d~t~, ~n~lyze the d~t~ from ;;m~zon SQS with  Kinesis, ~nd s~ve the results to ~n ;;m~zon Redshift cluster.
  D. Use ~n ;;m~zon ;;PI G~tew~y to put requests into ~n ;;m~zon SQS queue, ~n~lyze the d~t~ with ~n ;;WS  L~mbd~ function, ~nd s~ve the results to ~n ;;m~zon  Redshift cluster using ;;m~zon  EMR.

 Correct ;;nswer: B
 B (100%)

 Question #240
 ;; solutions ~rchitect needs to de ne ~ reference ~rchitecture for ~ solution for three-tier ~pplic~tions with web. ~pplic~tion, ~nd  NoSQL d~t~ l~yers. The reference ~rchitecture must meet the following requirements: •  High ~v~il~bility within ~n ;;WS  Region • ;;ble to f~il over in  1 minute to ~nother ;;WS  Region for dis~ster recovery •  Provide the most e cient solution while minimizing the imp~ct on the user experience Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Use ~n ;;m~zon  Route 53 weighted routing policy set to  100/0 ~cross the two selected  Regions. Set Time to  Live (TTL) to  1 hour.
  B. Use ~n ;;m~zon  Route 53 f~ilover routing policy for f~ilover from the prim~ry  Region to the dis~ster recovery  Region. Set Time to  Live (TTL) to 30 seconds.
  C. Use ~ glob~l t~ble within ;;m~zon  Dyn~moDB so d~t~ c~n be ~ccessed in the two selected  Regions.
  D.  B~ck up d~t~ from ~n ;;m~zon  Dyn~moDB t~ble in the prim~ry  Region every 60 minutes ~nd then write the d~t~ to ;;m~zon S3. Use S3 cross-Region replic~tion to copy the d~t~ from the prim~ry  Region to the dis~ster recovery  Region.  H~ve ~ script import the d~t~ into Dyn~moDB in ~ dis~ster recovery scen~rio.
  E.  Implement ~ hot st~ndby model using ;;uto Sc~ling groups for the web ~nd ~pplic~tion l~yers ~cross multiple ;;v~il~bility Zones in the Regions. Use zon~l  Reserved  Inst~nces for the minimum number of servers ~nd On-Dem~nd  Inst~nces for ~ny ~ddition~l resources.
  F. Use ;;uto Sc~ling groups for the web ~nd ~pplic~tion l~yers ~cross multiple ;;v~il~bility Zones in the  Regions. Use Spot  Inst~nces for the required resources.

 Correct ;;nswer: FDE
 BCE (92%)                                    8%

 Question #241
 ;; comp~ny m~nuf~ctures sm~rt vehicles. The comp~ny uses ~ custom ~pplic~tion to collect vehicle d~t~. The vehicles use the  MQTT protocol to connect to the ~pplic~tion. The comp~ny processes the d~t~ in 5-minute interv~ls. The comp~ny then copies vehicle telem~tics d~t~ to on- premises stor~ge. Custom ~pplic~tions ~n~lyze this d~t~ to detect ~nom~lies. The number of vehicles th~t send d~t~ grows const~ntly.  Newer vehicles gener~te high volumes of d~t~. The on-premises stor~ge solution is not ~ble to sc~le for pe~k tr~ c, which results in d~t~ loss. The comp~ny must modernize the solution ~nd migr~te the solution to ;;WS to resolve the sc~ling ch~llenges. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Use ;;WS  IoT Greengr~ss to send the vehicle d~t~ to ;;m~zon  M~n~ged Stre~ming for ;;p~che  K~fk~ (;;m~zon  MSK). Cre~te ~n ;;p~che K~fk~ ~pplic~tion to store the d~t~ in ;;m~zon S3. Use ~ pretr~ined model in ;;m~zon S~geM~ker to detect ~nom~lies.
  B. Use ;;WS  IoT Core to receive the vehicle d~t~. Con gure rules to route d~t~ to ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m th~t stores the d~t~ in ;;m~zon S3. Cre~te ~n ;;m~zon  Kinesis  D~t~ ;;n~lytics ~pplic~tion th~t re~ds from the delivery stre~m to detect ~nom~lies.
  C. Use ;;WS  IoT  FleetWise to collect the vehicle d~t~. Send the d~t~ to ~n ;;m~zon  Kinesis d~t~ stre~m. Use ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m to store the d~t~ in ;;m~zon S3. Use the built-in m~chine le~rning tr~nsforms in ;;WS Glue to detect ~nom~lies.
  D. Use ;;m~zon  MQ for  R~bbitMQ to collect the vehicle d~t~. Send the d~t~ to ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m to store the d~t~ in ;;m~zon S3. Use ;;m~zon  Lookout for  Metrics to detect ~nom~lies.

 Correct ;;nswer: C
 B (82%)                                   Other

 Question #242
 During ~n ~udit, ~ security te~m discovered th~t ~ development te~m w~s putting  I;;M user secret ~ccess keys in their code ~nd then committing it to ~n ;;WS CodeCommit repository. The security te~m w~nts to ~utom~tic~lly  nd ~nd remedi~te inst~nces of this security vulner~bility. Which solution will ensure th~t the credenti~ls ~re ~ppropri~tely secured ~utom~tic~lly?
  ;;.  Run ~ script nightly using ;;WS Systems  M~n~ger  Run Comm~nd to se~rch for credenti~ls on the development inst~nces.  If found, use ;;WS Secrets  M~n~ger to rot~te the credenti~ls
  B. Use ~ scheduled ;;WS  L~mbd~ function to downlo~d ~nd sc~n the ~pplic~tion code from CodeCommit.  If credenti~ls ~re found, gener~te new credenti~ls ~nd store them in ;;WS  KMS.
  C. Con gure ;;m~zon  M~cie to sc~n for credenti~ls in CodeCommit repositories.  If credenti~ls ~re found, trigger ~n ;;WS  L~mbd~ function to dis~ble the credenti~ls ~nd notify the user.
  D. Con gure ~ CodeCommit trigger to invoke ~n ;;WS  L~mbd~ function to sc~n new code submissions for credenti~ls.  If credenti~ls ~re found, dis~ble them in ;;WS  I;;M ~nd notify the user.

 Correct ;;nswer: ;;
 D (88%)                                   12%

 Question #243
 ;; comp~ny h~s ~ d~t~ l~ke in ;;m~zon S3 th~t needs to be ~ccessed by hundreds of ~pplic~tions ~cross m~ny ;;WS ~ccounts. The comp~ny's inform~tion security policy st~tes th~t the S3 bucket must not be ~ccessed over the public internet ~nd th~t e~ch ~pplic~tion should h~ve the minimum permissions necess~ry to function. To meet these requirements, ~ solutions ~rchitect pl~ns to use ~n S3 ~ccess point th~t is restricted to speci c VPCs for e~ch ~pplic~tion. Which combin~tion of steps should the solutions ~rchitect t~ke to implement this solution? (Choose two.)
  ;;. Cre~te ~n S3 ~ccess point for e~ch ~pplic~tion in the ;;WS ~ccount th~t owns the S3 bucket. Con gure e~ch ~ccess point to be ~ccessible only from the ~pplic~tion’s VPC. Upd~te the bucket policy to require ~ccess from ~n ~ccess point.
  B. Cre~te ~n interf~ce endpoint for ;;m~zon S3 in e~ch ~pplic~tion's VPC. Con gure the endpoint policy to ~llow ~ccess to ~n S3 ~ccess point. Cre~te ~ VPC g~tew~y ~tt~chment for the S3 endpoint.
  C. Cre~te ~ g~tew~y endpoint for ;;m~zon S3 in e~ch ~pplic~tion's VPCon gure the endpoint policy to ~llow ~ccess to ~n S3 ~ccess point. Specify the route t~ble th~t is used to ~ccess the ~ccess point.
  D. Cre~te ~n S3 ~ccess point for e~ch ~pplic~tion in e~ch ;;WS ~ccount ~nd ~tt~ch the ~ccess points to the S3 bucket. Con gure e~ch ~ccess point to be ~ccessible only from the ~pplic~tion's VPC. Upd~te the bucket policy to require ~ccess from ~n ~ccess point.
  E. Cre~te ~ g~tew~y endpoint for ;;m~zon S3 in the d~t~ l~ke's VPC. ;;tt~ch ~n endpoint policy to ~llow ~ccess to the S3 bucket. Specify the route t~ble th~t is used to ~ccess the bucket.

 Correct ;;nswer: DB
 ;;C (71%)                           11%        Other

 Question #244
 ;; comp~ny h~s developed ~ hybrid solution between its d~t~ center ~nd ;;WS. The comp~ny uses ;;m~zon VPC ~nd ;;m~zon  EC2 inst~nces th~t send ~pplic~tion logs to ;;m~zon CloudW~tch. The  EC2 inst~nces re~d d~t~ from multiple rel~tion~l d~t~b~ses th~t ~re hosted on premises. The comp~ny w~nts to monitor which  EC2 inst~nces ~re connected to the d~t~b~ses in ne~r-re~l time. The comp~ny ~lre~dy h~s ~ monitoring solution th~t uses Splunk on premises. ;; solutions ~rchitect needs to determine how to send networking tr~ c to Splunk. How should the solutions ~rchitect meet these requirements?
  ;;.  En~ble VPC  ows logs, ~nd send them to CloudW~tch. Cre~te ~n ;;WS  L~mbd~ function to periodic~lly export the CloudW~tch logs to ~n ;;m~zon S3 bucket by using the pre-de ned export function. Gener~te ;;CCESS_KEY ~nd SECRET_KEY ;;WS credenti~ls. Con gure Splunk to pull the logs from the S3 bucket by using those credenti~ls.
  B. Cre~te ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m with Splunk ~s the destin~tion. Con gure ~ pre-processing ;;WS  L~mbd~ function with ~  Kinesis  D~t~  Firehose stre~m processor th~t extr~cts individu~l log events from records sent by CloudW~tch  Logs subscription  lters. En~ble VPC  ows logs, ~nd send them to CloudW~tch. Cre~te ~ CloudW~tch  Logs subscription th~t sends log events to the  Kinesis  D~t~ Firehose delivery stre~m.
  C. ;;sk the comp~ny to log every request th~t is m~de to the d~t~b~ses ~long with the  EC2 inst~nce  IP ~ddress.  Export the CloudW~tch logs to ~n ;;m~zon S3 bucket. Use ;;m~zon ;;then~ to query the logs grouped by d~t~b~se n~me.  Export ;;then~ results to ~nother S3 bucket.  Invoke ~n ;;WS  L~mbd~ function to ~utom~tic~lly send ~ny new  le th~t is put in the S3 bucket to Splunk.
  D. Send the CloudW~tch logs to ~n ;;m~zon  Kinesis d~t~ stre~m with ;;m~zon  Kinesis  D~t~ ;;n~lytics for SQL ;;pplic~tions. Con gure ~  1- minute sliding window to collect the events. Cre~te ~ SQL query th~t uses the ~nom~ly detection templ~te to monitor ~ny networking tr~ c ~nom~lies in ne~r-re~l time. Send the result to ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m with Splunk ~s the destin~tion.

 Correct ;;nswer: ;;
 B (100%)

 Question #245
 ;; comp~ny h~s  ve development te~ms th~t h~ve e~ch cre~ted  ve ;;WS ~ccounts to develop ~nd host ~pplic~tions. To tr~ck spending, the development te~ms log in to e~ch ~ccount every month, record the current cost from the ;;WS  Billing ~nd Cost  M~n~gement console, ~nd provide the inform~tion to the comp~ny's  n~nce te~m. The comp~ny h~s strict compli~nce requirements ~nd needs to ensure th~t resources ~re cre~ted only in ;;WS  Regions in the United St~tes. However, some resources h~ve been cre~ted in other  Regions. ;; solutions ~rchitect needs to implement ~ solution th~t gives the  n~nce te~m the ~bility to tr~ck ~nd consolid~te expenditures for ~ll the ~ccounts. The solution ~lso must ensure th~t the comp~ny c~n cre~te resources only in  Regions in the United St~tes. Which combin~tion of steps will meet these requirements in the  MOST oper~tion~lly e cient w~y? (Choose three.)
  ;;. Cre~te ~ new ~ccount to serve ~s ~ m~n~gement ~ccount. Cre~te ~n ;;m~zon S3 bucket for the  n~nce te~m. Use ;;WS Cost ~nd Us~ge Reports to cre~te monthly reports ~nd to store the d~t~ in the  n~nce te~m's S3 bucket.
  B. Cre~te ~ new ~ccount to serve ~s ~ m~n~gement ~ccount.  Deploy ~n org~niz~tion in ;;WS Org~niz~tions with ~ll fe~tures en~bled.  Invite ~ll the existing ~ccounts to the org~niz~tion.  Ensure th~t e~ch ~ccount ~ccepts the invit~tion.
  C. Cre~te ~n OU th~t includes ~ll the development te~ms. Cre~te ~n SCP th~t ~llows the cre~tion of resources only in  Regions th~t ~re in the United St~tes. ;;pply the SCP to the OU.
  D. Cre~te ~n OU th~t includes ~ll the development te~ms. Cre~te ~n SCP th~t denies the cre~tion of resources in  Regions th~t ~re outside the United St~tes. ;;pply the SCP to the OU.
  E. Cre~te ~n  I;;M role in the m~n~gement ~ccount. ;;tt~ch ~ policy th~t includes permissions to view the  Billing ~nd Cost  M~n~gement console. ;;llow the  n~nce te~m users to ~ssume the role. Use ;;WS Cost  Explorer ~nd the  Billing ~nd Cost  M~n~gement console to ~n~lyze cost.
  F. Cre~te ~n  I;;M role in e~ch ;;WS ~ccount. ;;tt~ch ~ policy th~t includes permissions to view the  Billing ~nd Cost  M~n~gement console. ;;llow the  n~nce te~m users to ~ssume the role.

 Correct ;;nswer: ;;CF
 BDE (80%)                              12%      8%

 Question #246
 ;; comp~ny needs to cre~te ~nd m~n~ge multiple ;;WS ~ccounts for ~ number of dep~rtments from ~ centr~l loc~tion. The security te~m requires re~d-only ~ccess to ~ll ~ccounts from its own ;;WS ~ccount. The comp~ny is using ;;WS Org~niz~tions ~nd cre~ted ~n ~ccount for the security te~m. How should ~ solutions ~rchitect meet these requirements?
  ;;. Use the Org~niz~tion;;ccount;;ccessRole  I;;M role to cre~te ~ new  I;;M policy with re~d-only ~ccess in e~ch member ~ccount.  Est~blish ~ trust rel~tionship between the  I;;M policy in e~ch member ~ccount ~nd the security ~ccount. ;;sk the security te~m to use the  I;;M policy to g~in ~ccess.
  B. Use the Org~niz~tion;;ccount;;ccessRole  I;;M role to cre~te ~ new  I;;M role with re~d-only ~ccess in e~ch member ~ccount.  Est~blish ~ trust rel~tionship between the  I;;M role in e~ch member ~ccount ~nd the security ~ccount. ;;sk the security te~m to use the  I;;M role to g~in ~ccess.
  C. ;;sk the security te~m to use ;;WS Security Token Service (;;WS STS) to c~ll the ;;ssumeRole ;;PI for the Org~niz~tion;;ccount;;ccessRole I;;M role in the m~n~gement ~ccount from the security ~ccount. Use the gener~ted tempor~ry credenti~ls to g~in ~ccess.
  D. ;;sk the security te~m to use ;;WS Security Token Service (;;WS STS) to c~ll the ;;ssumeRole ;;PI for the Org~niz~tion;;ccount;;ccessRole I;;M role in the member ~ccount from the security ~ccount. Use the gener~ted tempor~ry credenti~ls to g~in ~ccess.

 Correct ;;nswer: B
 B (100%)

 Question #247
 ;; l~rge comp~ny runs worklo~ds in VPCs th~t ~re deployed ~cross hundreds of ;;WS ~ccounts.  E~ch VPC consists of public subnets ~nd priv~te subnets th~t sp~n ~cross multiple ;;v~il~bility Zones.  N;;T g~tew~ys ~re deployed in the public subnets ~nd ~llow outbound connectivity to the internet from the priv~te subnets. ;; solutions ~rchitect is working on ~ hub-~nd-spoke design. ;;ll priv~te subnets in the spoke VPCs must route tr~ c to the internet through ~n egress VPC. The solutions ~rchitect ~lre~dy h~s deployed ~  N;;T g~tew~y in ~n egress VPC in ~ centr~l ;;WS ~ccount. Which set of ~ddition~l steps should the solutions ~rchitect t~ke to meet these requirements?
  ;;. Cre~te peering connections between the egress VPC ~nd the spoke VPCs. Con gure the required routing to ~llow ~ccess to the internet.
  B. Cre~te ~ tr~nsit g~tew~y, ~nd sh~re it with the existing ;;WS ~ccounts. ;;tt~ch existing VPCs to the tr~nsit g~tew~y. Con gure the required routing to ~llow ~ccess to the internet.
  C. Cre~te ~ tr~nsit g~tew~y in every ~ccount. ;;tt~ch the  N;;T g~tew~y to the tr~nsit g~tew~ys. Con gure the required routing to ~llow ~ccess to the internet.
  D. Cre~te ~n ;;WS  Priv~teLink connection between the egress VPC ~nd the spoke VPCs. Con gure the required routing to ~llow ~ccess to the internet.

 Correct ;;nswer: ;;
 B (100%)

 Question #248
 ;;n educ~tion comp~ny is running ~ web ~pplic~tion used by college students ~round the world. The ~pplic~tion runs in ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster in ~n ;;uto Sc~ling group behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). ;; system ~dministr~tor detects ~ weekly spike in the number of f~iled login ~ttempts, which overwhelm the ~pplic~tion's ~uthentic~tion service. ;;ll the f~iled login ~ttempts origin~te from ~bout 500 different  IP ~ddresses th~t ch~nge e~ch week. ;; solutions ~rchitect must prevent the f~iled login ~ttempts from overwhelming the ~uthentic~tion service. Which solution meets these requirements with the  MOST oper~tion~l e ciency?
  ;;. Use ;;WS  Firew~ll  M~n~ger to cre~te ~ security group ~nd security group policy to deny ~ccess from the  IP ~ddresses.
  B. Cre~te ~n ;;WS W;;F web ;;CL with ~ r~te-b~sed rule, ~nd set the rule ~ction to  Block. Connect the web ;;CL to the ;;LB.
  C. Use ;;WS  Firew~ll  M~n~ger to cre~te ~ security group ~nd security group policy to ~llow ~ccess only to speci c CIDR r~nges.
  D. Cre~te ~n ;;WS W;;F web ;;CL with ~n  IP set m~tch rule, ~nd set the rule ~ction to  Block. Connect the web ;;CL to the ;;LB.

 Correct ;;nswer: B
 B (100%)

 Question #249
 ;; comp~ny oper~tes ~n on-premises softw~re-~s-~-service (S~~S) solution th~t ingests sever~l  les d~ily. The comp~ny provides multiple public SFTP endpoints to its customers to f~cilit~te the  le tr~nsfers. The customers ~dd the SFTP endpoint  IP ~ddresses to their  rew~ll ~llow list for outbound tr~ c. Ch~nges to the SFTP endpoint  IP ~ddresses ~re not permitted. The comp~ny w~nts to migr~te the S~~S solution to ;;WS ~nd decre~se the oper~tion~l overhe~d of the  le tr~nsfer service. Which solution meets these requirements?
  ;;.  Register the customer-owned block of  IP ~ddresses in the comp~ny's ;;WS ~ccount. Cre~te  El~stic  IP ~ddresses from the ~ddress pool ~nd ~ssign them to ~n ;;WS Tr~nsfer for SFTP endpoint. Use ;;WS Tr~nsfer to store the  les in ;;m~zon S3.
  B. ;;dd ~ subnet cont~ining the customer-owned block of  IP ~ddresses to ~ VPC. Cre~te  El~stic  IP ~ddresses from the ~ddress pool ~nd ~ssign them to ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB).  L~unch  EC2 inst~nces hosting  FTP services in ~n ;;uto Sc~ling group behind the ;;LStore the  les in ~tt~ched ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes.
  C.  Register the customer-owned block of  IP ~ddresses with ;;m~zon  Route 53. Cre~te ~li~s records in  Route 53 th~t point to ~  Network  Lo~d B~l~ncer (NLB).  L~unch  EC2 inst~nces hosting  FTP services in ~n ;;uto Sc~ling group behind the  NLB. Store the  les in ;;m~zon S3.
  D.  Register the customer-owned block of  IP ~ddresses in the comp~ny’s ;;WS ~ccount. Cre~te  El~stic  IP ~ddresses from the ~ddress pool ~nd ~ssign them to ~n ;;m~zon S3 VPC endpoint.  En~ble SFTP support on the S3 bucket.

 Correct ;;nswer: D
 ;; (100%)

 Question #250
 ;; comp~ny h~s ~ new ~pplic~tion th~t needs to run on  ve ;;m~zon  EC2 inst~nces in ~ single ;;WS  Region. The ~pplic~tion requires high- throughput, low-l~tency network connections between ~ll of the  EC2 inst~nces where the ~pplic~tion will run. There is no requirement for the ~pplic~tion to be f~ult toler~nt. Which solution will meet these requirements?
  ;;.  L~unch  ve new  EC2 inst~nces into ~ cluster pl~cement group.  Ensure th~t the  EC2 inst~nce type supports enh~nced networking.
  B.  L~unch  ve new  EC2 inst~nces into ~n ;;uto Sc~ling group in the s~me ;;v~il~bility Zone. ;;tt~ch ~n extr~ el~stic network interf~ce to e~ch EC2 inst~nce.
  C.  L~unch  ve new  EC2 inst~nces into ~ p~rtition pl~cement group.  Ensure th~t the  EC2 inst~nce type supports enh~nced networking.
  D.  L~unch  ve new  EC2 inst~nces into ~ spre~d pl~cement group. ;;tt~ch ~n extr~ el~stic network interf~ce to e~ch  EC2 inst~nce.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #251
 ;; comp~ny is cre~ting ~  REST ;;PI to sh~re inform~tion with six of its p~rtners b~sed in the United St~tes. The comp~ny h~s cre~ted ~n ;;m~zon ;;PI G~tew~y  Region~l endpoint.  E~ch of the six p~rtners will ~ccess the ;;PI once per d~y to post d~ily s~les  gures. ;;fter initi~l deployment, the comp~ny observes  1,000 requests per second origin~ting from 500 different  IP ~ddresses ~round the world. The comp~ny believes this tr~ c is origin~ting from ~ botnet ~nd w~nts to secure its ;;PI while minimizing cost. Which ~ppro~ch should the comp~ny t~ke to secure its ;;PI?
  ;;. Cre~te ~n ;;m~zon CloudFront distribution with the ;;PI ~s the origin. Cre~te ~n ;;WS W;;F web ;;CL with ~ rule to block clients th~t submit more th~n  ve requests per d~y. ;;ssoci~te the web ;;CL with the CloudFront distribution. Con gure CloudFront with ~n origin ~ccess identity (O;;I) ~nd ~ssoci~te it with the distribution. Con gure ;;PI G~tew~y to ensure only the O;;I c~n run the  POST method.
  B. Cre~te ~n ;;m~zon CloudFront distribution with the ;;PI ~s the origin. Cre~te ~n ;;WS W;;F web ;;CL with ~ rule to block clients th~t submit more th~n  ve requests per d~y. ;;ssoci~te the web ;;CL with the CloudFront distribution. ;;dd ~ custom he~der to the CloudFront distribution popul~ted with ~n ;;PI key. Con gure the ;;PI to require ~n ;;PI key on the  POST method.
  C. Cre~te ~n ;;WS W;;F web ;;CL with ~ rule to ~llow ~ccess to the  IP ~ddresses used by the six p~rtners. ;;ssoci~te the web ;;CL with the ;;PI. Cre~te ~ resource policy with ~ request limit ~nd ~ssoci~te it with the ;;PI. Con gure the ;;PI to require ~n ;;PI key on the  POST method.
  D. Cre~te ~n ;;WS W;;F web ;;CL with ~ rule to ~llow ~ccess to the  IP ~ddresses used by the six p~rtners. ;;ssoci~te the web ;;CL with the ;;PI. Cre~te ~ us~ge pl~n with ~ request limit ~nd ~ssoci~te it with the ;;PI. Cre~te ~n ;;PI key ~nd ~dd it to the us~ge pl~n.

 Correct ;;nswer: C
 D (94%)                                    6%

 Question #252
 ;; comp~ny uses ~n ;;m~zon ;;uror~  PostgreSQL  DB cluster for ~pplic~tions in ~ single ;;WS  Region. The comp~ny's d~t~b~se te~m must monitor ~ll d~t~ ~ctivity on ~ll the d~t~b~ses. Which solution will ~chieve this go~l?
  ;;. Set up ~n ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) ch~nge d~t~ c~pture (CDC) t~sk. Specify the ;;uror~  DB cluster ~s the source. Specify ;;m~zon  Kinesis  D~t~  Firehose ~s the t~rget. Use  Kinesis  D~t~  Firehose to uplo~d the d~t~ into ~n ;;m~zon OpenSe~rch Service cluster for further ~n~lysis.
  B. St~rt ~ d~t~b~se ~ctivity stre~m on the ;;uror~  DB cluster to c~pture the ~ctivity stre~m in ;;m~zon  EventBridge.  De ne ~n ;;WS  L~mbd~ function ~s ~ t~rget for  EventBridge.  Progr~m the  L~mbd~ function to decrypt the mess~ges from  EventBridge ~nd to publish ~ll d~t~b~se ~ctivity to ;;m~zon S3 for further ~n~lysis.
  C. St~rt ~ d~t~b~se ~ctivity stre~m on the ;;uror~  DB cluster to push the ~ctivity stre~m to ~n ;;m~zon  Kinesis d~t~ stre~m. Con gure ;;m~zon Kinesis  D~t~  Firehose to consume the  Kinesis d~t~ stre~m ~nd to deliver the d~t~ to ;;m~zon S3 for further ~n~lysis.
  D. Set up ~n ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) ch~nge d~t~ c~pture (CDC) t~sk. Specify the ;;uror~  DB cluster ~s the source. Specify ;;m~zon  Kinesis  D~t~  Firehose ~s the t~rget. Use  Kinesis  D~t~  Firehose to uplo~d the d~t~ into ~n ;;m~zon  Redshift cluster.  Run queries on the ;;m~zon  Redshift d~t~ to determine d~t~b~se ~ctivities on the ;;uror~ d~t~b~se.

 Correct ;;nswer: D
 C (100%)

 Question #253
 ;;n entert~inment comp~ny recently l~unched ~ new g~me. To ensure ~ good experience for pl~yers during the l~unch period, the comp~ny deployed ~ st~tic qu~ntity of  12 r6g.16xl~rge (memory optimized) ;;m~zon  EC2 inst~nces behind ~  Network  Lo~d  B~l~ncer. The comp~ny's oper~tions te~m used the ;;m~zon CloudW~tch ~gent ~nd ~ custom metric to include memory utiliz~tion in its monitoring str~tegy. ;;n~lysis of the CloudW~tch metrics from the l~unch period showed consumption ~t ~bout one qu~rter of the CPU ~nd memory th~t the comp~ny expected.  Initi~l dem~nd for the g~me h~s subsided ~nd h~s become more v~ri~ble. The comp~ny decides to use ~n ;;uto Sc~ling group th~t monitors the CPU ~nd memory consumption to dyn~mic~lly sc~le the inst~nce  eet. ;; solutions ~rchitect needs to con gure the ;;uto Sc~ling group to meet dem~nd in the most cost-effective w~y. Which solution will meet these requirements?
  ;;. Con gure the ;;uto Sc~ling group to deploy c6g.4xl~rge (compute optimized) inst~nces. Con gure ~ minimum c~p~city of 3, ~ desired c~p~city of 3, ~nd ~ m~ximum c~p~city of  12.
  B. Con gure the ;;uto Sc~ling group to deploy m6g.4xl~rge (gener~l purpose) inst~nces. Con gure ~ minimum c~p~city of 3, ~ desired c~p~city of 3, ~nd ~ m~ximum c~p~city of  12.
  C. Con gure the ;;uto Sc~ling group to deploy r6g.4xl~rge (memory optimized) inst~nces. Con gure ~ minimum c~p~city of 3, ~ desired c~p~city of 3, ~nd ~ m~ximum c~p~city of  12.
  D. Con gure the ;;uto Sc~ling group to deploy r6g.8xl~rge (memory optimized) inst~nces. Con gure ~ minimum c~p~city of 2, ~ desired c~p~city of 2, ~nd ~ m~ximum c~p~city of 6.

 Correct ;;nswer: D
 C (94%)                                   6%

 Question #254
 ;;  n~nci~l services comp~ny lo~ded millions of historic~l stock tr~des into ~n ;;m~zon  Dyn~moDB t~ble. The t~ble uses on-dem~nd c~p~city mode. Once e~ch d~y ~t midnight, ~ few million new records ~re lo~ded into the t~ble. ;;pplic~tion re~d ~ctivity ~g~inst the t~ble h~ppens in bursts throughout the d~y. ~nd ~ limited set of keys ~re repe~tedly looked up. The comp~ny needs to reduce costs ~ssoci~ted with  Dyn~moDB. Which str~tegy should ~ solutions ~rchitect recommend to meet this requirement?
  ;;.  Deploy ~n ;;m~zon  El~stiC~che cluster in front of the  Dyn~moDB t~ble
  B.  Deploy  Dyn~moDB ;;cceler~tor (D;;X). Con gure  Dyn~moDB ~uto sc~ling.  Purch~se S~vings  Pl~ns in Cost  Explorer.
  C. Use provisioned c~p~city mode.  Purch~se S~vings  Pl~ns in Cost  Explorer.
  D.  Deploy  Dyn~moDB ;;cceler~tor (D;;X). Use provisioned c~p~city mode. Con gure  Dyn~moDB ~uto sc~ling.

 Correct ;;nswer: ;;
 D (82%)                                  Other

 Question #255
 ;; comp~ny is cre~ting ~ centr~lized logging service running on ;;m~zon  EC2 th~t will receive ~nd ~n~lyze logs from hundreds of ;;WS ~ccounts. ;;WS  Priv~teLink is being used to provide connectivity between the client services ~nd the logging service. In e~ch ;;WS ~ccount with ~ client, ~n interf~ce endpoint h~s been cre~ted for the logging service ~nd is ~v~il~ble. The logging service running on EC2 inst~nces with ~  Network  Lo~d  B~l~ncer (NLB) ~re deployed in different subnets. The clients ~re un~ble to submit logs using the VPC endpoint. Which combin~tion of steps should ~ solutions ~rchitect t~ke to resolve this issue? (Choose two.)
  ;;. Check th~t the  N;;CL is ~tt~ched to the logging service subnet to ~llow communic~tions to ~nd from the  NLB subnets. Check th~t the  N;;CL is ~tt~ched to the  NLB subnet to ~llow communic~tions to ~nd from the logging service subnets running on  EC2 inst~nces.
  B. Check th~t the  N;;CL is ~tt~ched to the logging service subnets to ~llow communic~tions to ~nd from the interf~ce endpoint subnets. Check th~t the  N;;CL is ~tt~ched to the interf~ce endpoint subnet to ~llow communic~tions to ~nd from the logging service subnets running on  EC2 inst~nces.
  C. Check the security group for the logging service running on the  EC2 inst~nces to ensure it ~llows ingress from the  NLB subnets.
  D. Check the security group for the logging service running on  EC2 inst~nces to ensure it ~llows ingress from the clients.
  E. Check the security group for the  NLB to ensure it ~llows ingress from the interf~ce endpoint subnets.

 Correct ;;nswer: ;;C
 ;;C (57%)                            BD (30%)            11%

 Question #256
 ;; comp~ny h~s millions of objects in ~n ;;m~zon S3 bucket. The objects ~re in the S3 St~nd~rd stor~ge cl~ss. ;;ll the S3 objects ~re ~ccessed frequently. The number of users ~nd ~pplic~tions th~t ~ccess the objects is incre~sing r~pidly. The objects ~re encrypted with server-side encryption with ;;WS  KMS keys (SSE-KMS). ;; solutions ~rchitect reviews the comp~ny’s monthly ;;WS invoice ~nd notices th~t ;;WS  KMS costs ~re incre~sing bec~use of the high number of requests from ;;m~zon S3. The solutions ~rchitect needs to optimize costs with minim~l ch~nges to the ~pplic~tion. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ new S3 bucket th~t h~s server-side encryption with customer-provided keys (SSE-C) ~s the encryption type. Copy the existing objects to the new S3 bucket. Specify SSE-C.
  B. Cre~te ~ new S3 bucket th~t h~s server-side encryption with ;;m~zon S3 m~n~ged keys (SSE-S3) ~s the encryption type. Use S3  B~tch Oper~tions to copy the existing objects to the new S3 bucket. Specify SSE-S3.
  C. Use ;;WS CloudHSM to store the encryption keys. Cre~te ~ new S3 bucket. Use S3  B~tch Oper~tions to copy the existing objects to the new S3 bucket.  Encrypt the objects by using the keys from CloudHSM.
  D. Use the S3  Intelligent-Tiering stor~ge cl~ss for the S3 bucket. Cre~te ~n S3  Intelligent-Tiering ~rchive con gur~tion to tr~nsition objects th~t ~re not ~ccessed for 90 d~ys to S3 Gl~cier  Deep ;;rchive.

 Correct ;;nswer: ;;
 B (100%)

 Question #257
 ;; medi~ stor~ge ~pplic~tion uplo~ds user photos to ;;m~zon S3 for processing by ;;WS  L~mbd~ functions. ;;pplic~tion st~te is stored in ;;m~zon Dyn~moDB t~bles. Users ~re reporting th~t some uplo~ded photos ~re not being processed properly. The ~pplic~tion developers tr~ce the logs ~nd  nd th~t  L~mbd~ is experiencing photo processing issues when thous~nds of users uplo~d photos simult~neously. The issues ~re the result of L~mbd~ concurrency limits ~nd the perform~nce of  Dyn~moDB when d~t~ is s~ved. Which combin~tion of ~ctions should ~ solutions ~rchitect t~ke to incre~se the perform~nce ~nd reli~bility of the ~pplic~tion? (Choose two.)
  ;;.  Ev~lu~te ~nd ~djust the  RCUs for the  Dyn~moDB t~bles.
  B.  Ev~lu~te ~nd ~djust the WCUs for the  Dyn~moDB t~bles.
  C. ;;dd ~n ;;m~zon  El~stiC~che l~yer to incre~se the perform~nce of  L~mbd~ functions.
  D. ;;dd ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue ~nd reprocessing logic between ;;m~zon S3 ~nd the  L~mbd~ functions.
  E. Use S3 Tr~nsfer ;;cceler~tion to provide lower l~tency to users.

 Correct ;;nswer: BD
 BD (100%)

 Question #258
 ;; comp~ny runs ~n ~pplic~tion in ~n on-premises d~t~ center. The ~pplic~tion gives users the ~bility to uplo~d medi~  les. The  les persist in ~  le server. The web ~pplic~tion h~s m~ny users. The ~pplic~tion server is overutilized, which c~uses d~t~ uplo~ds to f~il occ~sion~lly. The comp~ny frequently ~dds new stor~ge to the  le server. The comp~ny w~nts to resolve these ch~llenges by migr~ting the ~pplic~tion to ;;WS. Users from ~cross the United St~tes ~nd C~n~d~ ~ccess the ~pplic~tion. Only ~uthentic~ted users should h~ve the ~bility to ~ccess the ~pplic~tion to uplo~d  les. The comp~ny will consider ~ solution th~t ref~ctors the ~pplic~tion, ~nd the comp~ny needs to ~cceler~te ~pplic~tion development. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Use ;;WS ;;pplic~tion  Migr~tion Service to migr~te the ~pplic~tion server to ;;m~zon  EC2 inst~nces. Cre~te ~n ;;uto Sc~ling group for the EC2 inst~nces. Use ~n ;;pplic~tion  Lo~d  B~l~ncer to distribute the requests.  Modify the ~pplic~tion to use ;;m~zon S3 to persist the  les. Use ;;m~zon Cognito to ~uthentic~te users.
  B. Use ;;WS ;;pplic~tion  Migr~tion Service to migr~te the ~pplic~tion server to ;;m~zon  EC2 inst~nces. Cre~te ~n ;;uto Sc~ling group for the EC2 inst~nces. Use ~n ;;pplic~tion  Lo~d  B~l~ncer to distribute the requests. Set up ;;WS  I;;M  Identity Center (;;WS Single Sign-On) to give users the ~bility to sign in to the ~pplic~tion.  Modify the ~pplic~tion to use ;;m~zon S3 to persist the  les.
  C. Cre~te ~ st~tic website for uplo~ds of medi~  les. Store the st~tic ~ssets in ;;m~zon S3. Use ;;WS ;;ppSync to cre~te ~n ;;PI. Use ;;WS L~mbd~ resolvers to uplo~d the medi~  les to ;;m~zon S3. Use ;;m~zon Cognito to ~uthentic~te users.
  D. Use ;;WS ;;mplify to cre~te ~ st~tic website for uplo~ds of medi~  les. Use ;;mplify  Hosting to serve the website through ;;m~zon CloudFront. Use ;;m~zon S3 to store the uplo~ded medi~  les. Use ;;m~zon Cognito to ~uthentic~te users.

 Correct ;;nswer: ;;
 D (90%)                                    10%

 Question #259
 ;; comp~ny h~s ~n ~pplic~tion th~t is deployed on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The inst~nces ~re p~rt of ~n ;;uto Sc~ling group. The ~pplic~tion h~s unpredict~ble worklo~ds ~nd frequently sc~les out ~nd in. The comp~ny’s development te~m w~nts to ~n~lyze ~pplic~tion logs to  nd w~ys to improve the ~pplic~tion's perform~nce.  However, the logs ~re no longer ~v~il~ble ~fter inst~nces sc~le in. Which solution will give the development te~m the ~bility to view the ~pplic~tion logs ~fter ~ sc~le-in event?
  ;;.  En~ble ~ccess logs for the ;;LB. Store the logs in ~n ;;m~zon S3 bucket.
  B. Con gure the  EC2 inst~nces to publish logs to ;;m~zon CloudW~tch  Logs by using the uni ed CloudW~tch ~gent.
  C.  Modify the ;;uto Sc~ling group to use ~ step sc~ling policy.
  D.  Instrument the ~pplic~tion with ;;WS X-R~y tr~cing.

 Correct ;;nswer: B
 B (100%)

 Question #260
 ;; comp~ny runs ~n un~uthentic~ted st~tic website (www.ex~mple.com) th~t includes ~ registr~tion form for users. The website uses ;;m~zon S3 for hosting ~nd uses ;;m~zon CloudFront ~s the content delivery network with ;;WS W;;F con gured. When the registr~tion form is submitted, the website c~lls ~n ;;m~zon ;;PI G~tew~y ;;PI endpoint th~t invokes ~n ;;WS  L~mbd~ function to process the p~ylo~d ~nd forw~rd the p~ylo~d to ~n extern~l ;;PI c~ll. During testing, ~ solutions ~rchitect encounters ~ cross-origin resource sh~ring (CORS) error. The solutions ~rchitect con rms th~t the CloudFront distribution origin h~s the ;;ccess-Control-;;llow-Origin he~der set to www.ex~mple.com. Wh~t should the solutions ~rchitect do to resolve the error?
  ;;. Ch~nge the CORS con gur~tion on the S3 bucket. ;;dd rules for CORS to the ;;llowedOrigin element for www.ex~mple.com.
  B.  En~ble the CORS setting in ;;WS W;;F. Cre~te ~ web ;;CL rule in which the ;;ccess-Control-;;llow-Origin he~der is set to www.ex~mple.com.
  C.  En~ble the CORS setting on the ;;PI G~tew~y ;;PI endpoint.  Ensure th~t the ;;PI endpoint is con gured to return ~ll responses th~t h~ve the ;;ccess-Control-;;llow-Origin he~der set to www.ex~mple.com.
  D.  En~ble the CORS setting on the  L~mbd~ function.  Ensure th~t the return code of the function h~s the ;;ccess-Control-;;llow-Origin he~der set to www.ex~mple.com.

 Correct ;;nswer: B
 C (94%)                                   6%

 Question #261
 ;; comp~ny h~s m~ny sep~r~te ;;WS ~ccounts ~nd uses no centr~l billing or m~n~gement.  E~ch ;;WS ~ccount hosts services for different dep~rtments in the comp~ny. The comp~ny h~s ~  Microsoft ;;zure ;;ctive  Directory th~t is deployed. ;; solutions ~rchitect needs to centr~lize billing ~nd m~n~gement of the comp~ny’s ;;WS ~ccounts. The comp~ny w~nts to st~rt using identity feder~tion inste~d of m~nu~l user m~n~gement. The comp~ny ~lso w~nts to use tempor~ry credenti~ls inste~d of long-lived ~ccess keys. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Cre~te ~ new ;;WS ~ccount to serve ~s ~ m~n~gement ~ccount.  Deploy ~n org~niz~tion in ;;WS Org~niz~tions.  Invite e~ch existing ;;WS ~ccount to join the org~niz~tion.  Ensure th~t e~ch ~ccount ~ccepts the invit~tion.
  B. Con gure e~ch ;;WS ~ccount's em~il ~ddress to be ~ws+@ex~mple.com so th~t ~ccount m~n~gement em~il mess~ges ~nd invoices ~re sent to the s~me pl~ce.
  C.  Deploy ;;WS  I;;M  Identity Center (;;WS Single Sign-On) in the m~n~gement ~ccount. Connect  I;;M  Identity Center to the ;;zure ;;ctive Directory. Con gure  I;;M  Identity Center for ~utom~tic synchroniz~tion of users ~nd groups.
  D.  Deploy ~n ;;WS  M~n~ged  Microsoft ;;D directory in the m~n~gement ~ccount. Sh~re the directory with ~ll other ~ccounts in the org~niz~tion by using ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M).
  E. Cre~te ;;WS  I;;M  Identity Center (;;WS Single Sign-On) permission sets. ;;tt~ch the permission sets to the ~ppropri~te  I;;M  Identity Center groups ~nd ;;WS ~ccounts.
  F. Con gure ;;WS  Identity ~nd ;;ccess  M~n~gement (I;;M) in e~ch ;;WS ~ccount to use ;;WS  M~n~ged  Microsoft ;;D for ~uthentic~tion ~nd ~uthoriz~tion.

 Correct ;;nswer: CDE
 ;;CE (100%)

 Question #262
 ;; comp~ny w~nts to m~n~ge the costs ~ssoci~ted with ~ group of 20 ~pplic~tions th~t ~re infrequently used, but ~re still business-critic~l, by migr~ting to ;;WS. The ~pplic~tions ~re ~ mix of J~v~ ~nd  Node.js spre~d ~cross different inst~nce clusters. The comp~ny w~nts to minimize costs while st~nd~rdizing by using ~ single deployment methodology. Most of the ~pplic~tions ~re p~rt of month-end processing routines with ~ sm~ll number of concurrent users, but they ~re occ~sion~lly run ~t other times. ;;ver~ge ~pplic~tion memory consumption is less th~n  1 GB. though some ~pplic~tions use ~s much ~s 2.5 GB of memory during pe~k processing. The most import~nt ~pplic~tion in the group is ~ billing report written in J~v~ th~t ~ccesses multiple d~t~ sources ~nd often runs for sever~l hours. Which is the  MOST cost-effective solution?
  ;;.  Deploy ~ sep~r~te ;;WS  L~mbd~ function for e~ch ~pplic~tion. Use ;;WS CloudTr~il logs ~nd ;;m~zon CloudW~tch ~l~rms to verify completion of critic~l jobs.
  B.  Deploy ;;m~zon  ECS cont~iners on ;;m~zon  EC2 with ;;uto Sc~ling con gured for memory utiliz~tion of 75%.  Deploy ~n  ECS t~sk for e~ch ~pplic~tion being migr~ted with  ECS t~sk sc~ling.  Monitor services ~nd hosts by using ;;m~zon CloudW~tch.
  C.  Deploy ;;WS  El~stic  Be~nst~lk for e~ch ~pplic~tion with ;;uto Sc~ling to ensure th~t ~ll requests h~ve su cient resources.  Monitor e~ch ;;WS  El~stic  Be~nst~lk deployment by using CloudW~tch ~l~rms.
  D.  Deploy ~ new ;;m~zon  EC2 inst~nce cluster th~t co-hosts ~ll ~pplic~tions by using  EC2 ;;uto Sc~ling ~nd ;;pplic~tion  Lo~d  B~l~ncers. Sc~le cluster size b~sed on ~ custom metric set on inst~nce memory utiliz~tion.  Purch~se 3-ye~r  Reserved  Inst~nce reserv~tions equ~l to the GroupM~xSize p~r~meter of the ;;uto Sc~ling group.

 Correct ;;nswer: B
 B (100%)

 Question #263
 ;; solutions ~rchitect needs to review the design of ~n ;;m~zon  EMR cluster th~t is using the  EMR  File System (EMRFS). The cluster performs t~sks th~t ~re critic~l to business needs. The cluster is running ;;m~zon  EC2 On-Dem~nd  Inst~nces ~t ~ll times for ~ll t~sk, prim~ry, ~nd core nodes. The  EMR t~sks run e~ch morning, st~rting ~t  1:00 ;;M. ~nd t~ke 6 hours to  nish running. The ~mount of time to complete the processing is not ~ priority bec~use the d~t~ is not referenced until l~te in the d~y. The solutions ~rchitect must review the ~rchitecture ~nd suggest ~ solution to minimize the compute costs. Which solution should the solutions ~rchitect recommend to meet these requirements?
  ;;.  L~unch ~ll t~sk, prim~ry, ~nd core nodes on Spot  Inst~nces in ~n inst~nce  eet. Termin~te the cluster, including ~ll inst~nces, when the processing is completed.
  B.  L~unch the prim~ry ~nd core nodes on On-Dem~nd  Inst~nces.  L~unch the t~sk nodes on Spot  Inst~nces in ~n inst~nce  eet. Termin~te the cluster, including ~ll inst~nces, when the processing is completed.  Purch~se Compute S~vings  Pl~ns to cover the On-Dem~nd  Inst~nce us~ge.
  C. Continue to l~unch ~ll nodes on On-Dem~nd  Inst~nces. Termin~te the cluster, including ~ll inst~nces, when the processing is completed. Purch~se Compute S~vings  Pl~ns to cover the On-Dem~nd  Inst~nce us~ge.
  D.  L~unch the prim~ry ~nd core nodes on On-Dem~nd  Inst~nces.  L~unch the t~sk nodes on Spot  Inst~nces in ~n inst~nce  eet. Termin~te only the t~sk node inst~nces when the processing is completed.  Purch~se Compute S~vings  Pl~ns to cover the On-Dem~nd  Inst~nce us~ge.

 Correct ;;nswer: C
 D (50%)                                  B (50%)

 Question #264
 ;; comp~ny h~s migr~ted ~ leg~cy ~pplic~tion to the ;;WS Cloud. The ~pplic~tion runs on three ;;m~zon  EC2 inst~nces th~t ~re spre~d ~cross three ;;v~il~bility Zones. One  EC2 inst~nce is in e~ch ;;v~il~bility Zone. The  EC2 inst~nces ~re running in three priv~te subnets of the VPC ~nd ~re set up ~s t~rgets for ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t is ~ssoci~ted with three public subnets. The ~pplic~tion needs to communic~te with on-premises systems. Only tr~ c from  IP ~ddresses in the comp~ny's  IP ~ddress r~nge ~re ~llowed to ~ccess the on-premises systems. The comp~ny’s security te~m is bringing only one  IP ~ddress from its intern~l  IP ~ddress r~nge to the cloud. The comp~ny h~s ~dded this  IP ~ddress to the ~llow list for the comp~ny  rew~ll. The comp~ny ~lso h~s cre~ted ~n  El~stic  IP ~ddress for this  IP ~ddress. ;; solutions ~rchitect needs to cre~te ~ solution th~t gives the ~pplic~tion the ~bility to communic~te with the on-premises systems. The solution ~lso must be ~ble to mitig~te f~ilures ~utom~tic~lly. Which solution will meet these requirements?
  ;;.  Deploy three  N;;T g~tew~ys, one in e~ch public subnet. ;;ssign the  El~stic  IP ~ddress to the  N;;T g~tew~ys. Turn on he~lth checks for the N;;T g~tew~ys.  If ~  N;;T g~tew~y f~ils ~ he~lth check, recre~te the  N;;T g~tew~y ~nd ~ssign the  El~stic  IP ~ddress to the new  N;;T g~tew~y.
  B.  Repl~ce the ;;LB with ~  Network  Lo~d  B~l~ncer (NLB). ;;ssign the  El~stic  IP ~ddress to the  NLTurn on he~lth checks for the  NLIn the c~se of ~ f~iled he~lth check, redeploy the  NLB in different subnets.
  C.  Deploy ~ single  N;;T g~tew~y in ~ public subnet. ;;ssign the  El~stic  IP ~ddress to the  N;;T g~tew~y. Use ;;m~zon CloudW~tch with ~ custom metric to monitor the  N;;T g~tew~y.  If the  N;;T g~tew~y is unhe~lthy, invoke ~n ;;WS  L~mbd~ function to cre~te ~ new  N;;T g~tew~y in ~ different subnet. ;;ssign the  El~stic  IP ~ddress to the new  N;;T g~tew~y.
  D. ;;ssign the  El~stic  IP ~ddress to the ;;LB. Cre~te ~n ;;m~zon  Route 53 simple record with the  El~stic  IP ~ddress ~s the v~lue. Cre~te ~  Route 53 he~lth check.  In the c~se of ~ f~iled he~lth check, recre~te the ;;LB in different subnets.

 Correct ;;nswer: ;;
 C (100%)

 Question #265
 ;; comp~ny uses ;;WS Org~niz~tions to m~n~ge more th~n  1,000 ;;WS ~ccounts. The comp~ny h~s cre~ted ~ new developer org~niz~tion. There ~re 540 developer member ~ccounts th~t must be moved to the new developer org~niz~tion. ;;ll ~ccounts ~re set up with ~ll the required inform~tion so th~t e~ch ~ccount c~n be oper~ted ~s ~ st~nd~lone ~ccount. Which combin~tion of steps should ~ solutions ~rchitect t~ke to move ~ll of the developer ~ccounts to the new developer org~niz~tion? (Choose three.)
  ;;. C~ll the  Move;;ccount oper~tion in the Org~niz~tions ;;PI from the old org~niz~tion's m~n~gement ~ccount to migr~te the developer ~ccounts to the new developer org~niz~tion.
  B.  From the m~n~gement ~ccount, remove e~ch developer ~ccount from the old org~niz~tion using the  Remove;;ccountFromOrg~niz~tion oper~tion in the Org~niz~tions ;;PI.
  C.  From e~ch developer ~ccount, remove the ~ccount from the old org~niz~tion using the  Remove;;ccountFromOrg~niz~tion oper~tion in the Org~niz~tions ;;PI.
  D. Sign in to the new developer org~niz~tion's m~n~gement ~ccount ~nd cre~te ~ pl~ceholder member ~ccount th~t ~cts ~s ~ t~rget for the developer ~ccount migr~tion.
  E. C~ll the  Invite;;ccountToOrg~niz~tion oper~tion in the Org~niz~tions ;;PI from the new developer org~niz~tion's m~n~gement ~ccount to send invit~tions to the developer ~ccounts.
  F.  H~ve e~ch developer sign in to their ~ccount ~nd con rm to join the new developer org~niz~tion.

 Correct ;;nswer: CEF
 BEF (85%)                                  Other

 Question #266
 ;; comp~ny’s inter~ctive web ~pplic~tion uses ~n ;;m~zon CloudFront distribution to serve im~ges from ~n ;;m~zon S3 bucket. Occ~sion~lly, third- p~rty tools ingest corrupted im~ges into the S3 bucket. This im~ge corruption c~uses ~ poor user experience in the ~pplic~tion l~ter. The comp~ny h~s successfully implemented ~nd tested  Python logic to detect corrupt im~ges. ;; solutions ~rchitect must recommend ~ solution to integr~te the detection logic with minim~l l~tency between the ingestion ~nd serving. Which solution will meet these requirements?
  ;;. Use ~  L~mbd~@Edge function th~t is invoked by ~ viewer-response event.
  B. Use ~  L~mbd~@Edge function th~t is invoked by ~n origin-response event.
  C. Use ~n S3 event noti c~tion th~t invokes ~n ;;WS  L~mbd~ function.
  D. Use ~n S3 event noti c~tion th~t invokes ~n ;;WS Step  Functions st~te m~chine.

 Correct ;;nswer: B
 C (100%)

 Question #267
 ;; comp~ny h~s ~n ~pplic~tion th~t runs on ;;m~zon  EC2 inst~nces in ~n ;;m~zon  EC2 ;;uto Sc~ling group. The comp~ny uses ;;WS CodePipeline to deploy the ~pplic~tion. The inst~nces th~t run in the ;;uto Sc~ling group ~re const~ntly ch~nging bec~use of sc~ling events. When the comp~ny deploys new ~pplic~tion code versions, the comp~ny inst~lls the ;;WS CodeDeploy ~gent on ~ny new t~rget  EC2 inst~nces ~nd ~ssoci~tes the inst~nces with the CodeDeploy deployment group. The ~pplic~tion is set to go live within the next 24 hours. Wh~t should ~ solutions ~rchitect recommend to ~utom~te the ~pplic~tion deployment process with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;. Con gure ;;m~zon  EventBridge to invoke ~n ;;WS  L~mbd~ function when ~ new  EC2 inst~nce is l~unched into the ;;uto Sc~ling group. Code the  L~mbd~ function to ~ssoci~te the  EC2 inst~nces with the CodeDeploy deployment group.
  B. Write ~ script to suspend ;;m~zon  EC2 ;;uto Sc~ling oper~tions before the deployment of new code. When the deployment is complete, cre~te ~ new ;;MI ~nd con gure the ;;uto Sc~ling group's l~unch templ~te to use the new ;;MI for new l~unches.  Resume ;;m~zon  EC2 ;;uto Sc~ling oper~tions.
  C. Cre~te ~ new ;;WS CodeBuild project th~t cre~tes ~ new ;;MI th~t cont~ins the new code. Con gure CodeBuild to upd~te the ;;uto Sc~ling group’s l~unch templ~te to the new ;;MI.  Run ~n ;;m~zon  EC2 ;;uto Sc~ling inst~nce refresh oper~tion.
  D. Cre~te ~ new ;;MI th~t h~s the CodeDeploy ~gent inst~lled. Con gure the ;;uto Sc~ling group’s l~unch templ~te to use the new ;;MI. ;;ssoci~te the CodeDeploy deployment group with the ;;uto Sc~ling group inste~d of the  EC2 inst~nces.

 Correct ;;nswer: D
 D (93%)                                    7%

 Question #268
 ;; comp~ny h~s ~ website th~t runs on four ;;m~zon  EC2 inst~nces th~t ~re behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). When the ;;LB detects th~t ~n  EC2 inst~nce is no longer ~v~il~ble, ~n ;;m~zon CloudW~tch ~l~rm enters the ;;L;;RM st~te. ;; member of the comp~ny's oper~tions te~m then m~nu~lly ~dds ~ new  EC2 inst~nce behind the ;;LB. ;; solutions ~rchitect needs to design ~ highly ~v~il~ble solution th~t ~utom~tic~lly h~ndles the repl~cement of  EC2 inst~nces. The comp~ny needs to minimize downtime during the switch to the new solution. Which set of steps should the solutions ~rchitect t~ke to meet these requirements?
  ;;.  Delete the existing ;;LB. Cre~te ~n ;;uto Sc~ling group th~t is con gured to h~ndle the web ~pplic~tion tr~ c. ;;tt~ch ~ new l~unch templ~te to the ;;uto Sc~ling group. Cre~te ~ new ;;LB. ;;tt~ch the ;;uto Sc~ling group to the new ;;LB. ;;tt~ch the existing  EC2 inst~nces to the ;;uto Sc~ling group.
  B. Cre~te ~n ;;uto Sc~ling group th~t is con gured to h~ndle the web ~pplic~tion tr~ c. ;;tt~ch ~ new l~unch templ~te to the ;;uto Sc~ling group. ;;tt~ch the ;;uto Sc~ling group to the existing ;;L;;tt~ch the existing  EC2 inst~nces to the ;;uto Sc~ling group.
  C.  Delete the existing ;;LB ~nd the  EC2 inst~nces. Cre~te ~n ;;uto Sc~ling group th~t is con gured to h~ndle the web ~pplic~tion tr~ c. ;;tt~ch ~ new l~unch templ~te to the ;;uto Sc~ling group. Cre~te ~ new ;;LB. ;;tt~ch the ;;uto Sc~ling group to the new ;;LB. W~it for the ;;uto Sc~ling group to l~unch the minimum number of  EC2 inst~nces.
  D. Cre~te ~n ;;uto Sc~ling group th~t is con gured to h~ndle the web ~pplic~tion tr~ c. ;;tt~ch ~ new l~unch templ~te to the ;;uto Sc~ling group. ;;tt~ch the ;;uto Sc~ling group to the existing ;;LB. W~it for the existing ;;LB to register the existing  EC2 inst~nces with the ;;uto Sc~ling group.

 Correct ;;nswer: C
 B (94%)                                     6%

 Question #269
 ;; comp~ny w~nts to optimize ;;WS d~t~-tr~nsfer costs ~nd compute costs ~cross developer ~ccounts within the comp~ny's org~niz~tion in ;;WS Org~niz~tions.  Developers c~n con gure VPCs ~nd l~unch ;;m~zon  EC2 inst~nces in ~ single ;;WS  Region. The  EC2 inst~nces retrieve ~pproxim~tely  1 TB of d~t~ e~ch d~y from ;;m~zon S3. The developer ~ctivity le~ds to excessive monthly d~t~-tr~nsfer ch~rges ~nd  N;;T g~tew~y processing ch~rges between  EC2 inst~nces ~nd S3 buckets, ~long with high compute costs. The comp~ny w~nts to pro~ctively enforce ~pproved ~rchitectur~l p~tterns for ~ny  EC2 inst~nce ~nd VPC infr~structure th~t developers deploy within the ;;WS ~ccounts. The comp~ny does not w~nt this enforcement to neg~tively ~ffect the speed ~t which the developers c~n perform their t~sks. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Cre~te SCPs to prevent developers from l~unching un~pproved  EC2 inst~nce types.  Provide the developers with ~n ;;WS CloudForm~tion templ~te to deploy ~n ~pproved VPC con gur~tion with S3 interf~ce endpoints. Scope the developers'  I;;M permissions so th~t the developers c~n l~unch VPC resources only with CloudForm~tion.
  B. Cre~te ~ d~ily forec~sted budget with ;;WS  Budgets to monitor  EC2 compute costs ~nd S3 d~t~-tr~nsfer costs ~cross the developer ~ccounts. When the forec~sted cost is 75% of the ~ctu~l budget cost, send ~n ~lert to the developer te~ms.  If the ~ctu~l budget cost is  100%, cre~te ~ budget ~ction to termin~te the developers'  EC2 inst~nces ~nd VPC infr~structure.
  C. Cre~te ~n ;;WS Service C~t~log portfolio th~t users c~n use to cre~te ~n ~pproved VPC con gur~tion with S3 g~tew~y endpoints ~nd ~pproved  EC2 inst~nces. Sh~re the portfolio with the developer ~ccounts. Con gure ~n ;;WS Service C~t~log l~unch constr~int to use ~n ~pproved  I;;M role. Scope the developers'  I;;M permissions to ~llow ~ccess only to ;;WS Service C~t~log.
  D. Cre~te ~nd deploy ;;WS Con g rules to monitor the compli~nce of  EC2 ~nd VPC resources in the developer ;;WS ~ccounts.  If developers l~unch un~pproved  EC2 inst~nces or if developers cre~te VPCs without S3 g~tew~y endpoints, perform ~ remedi~tion ~ction to termin~te the un~pproved resources.

 Correct ;;nswer: C
 C (100%)

 Question #270
 ;; comp~ny is exp~nding. The comp~ny pl~ns to sep~r~te its resources into hundreds of different ;;WS ~ccounts in multiple ;;WS  Regions. ;; solutions ~rchitect must recommend ~ solution th~t denies ~ccess to ~ny oper~tions outside of speci c~lly design~ted  Regions. Which solution will meet these requirements?
  ;;. Cre~te  I;;M roles for e~ch ~ccount. Cre~te  I;;M policies with condition~l ~llow permissions th~t include only ~pproved  Regions for the ~ccounts.
  B. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Cre~te  I;;M users for e~ch ~ccount. ;;tt~ch ~ policy to e~ch user to block ~ccess to  Regions where ~n ~ccount c~nnot deploy infr~structure.
  C.  L~unch ~n ;;WS Control Tower l~nding zone. Cre~te OUs ~nd ~tt~ch SCPs th~t deny ~ccess to run services outside of the ~pproved  Regions.
  D.  En~ble ;;WS Security  Hub in e~ch ~ccount. Cre~te controls to specify the  Regions where ~n ~ccount c~n deploy infr~structure.

 Correct ;;nswer: B
 C (100%)

 Question #271
 ;; comp~ny w~nts to ref~ctor its ret~il ordering web ~pplic~tion th~t currently h~s ~ lo~d-b~l~nced ;;m~zon  EC2 inst~nce  eet for web hosting, d~t~b~se ;;PI services, ~nd business logic. The comp~ny needs to cre~te ~ decoupled, sc~l~ble ~rchitecture with ~ mech~nism for ret~ining f~iled orders while ~lso minimizing oper~tion~l costs. Which solution will meet these requirements?
  ;;. Use ;;m~zon S3 for web hosting with ;;m~zon ;;PI G~tew~y for d~t~b~se ;;PI services. Use ;;m~zon Simple Queue Service (;;m~zon SQS) for order queuing. Use ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) for business logic with ;;m~zon SQS long polling for ret~ining f~iled orders.
  B. Use ;;WS  El~stic  Be~nst~lk for web hosting with ;;m~zon ;;PI G~tew~y for d~t~b~se ;;PI services. Use ;;m~zon  MQ for order queuing. Use ;;WS Step  Functions for business logic with ;;m~zon S3 Gl~cier  Deep ;;rchive for ret~ining f~iled orders.
  C. Use ;;m~zon S3 for web hosting with ;;WS ;;ppSync for d~t~b~se ;;PI services. Use ;;m~zon Simple Queue Service (;;m~zon SQS) for order queuing. Use ;;WS  L~mbd~ for business logic with ~n ;;m~zon SQS de~d-letter queue for ret~ining f~iled orders.
  D. Use ;;m~zon  Lights~il for web hosting with ;;WS ;;ppSync for d~t~b~se ;;PI services. Use ;;m~zon Simple  Em~il Service (;;m~zon SES) for order queuing. Use ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) for business logic with ;;m~zon OpenSe~rch Service for ret~ining f~iled orders.

 Correct ;;nswer: ;;
 C (92%)                                    8%

 Question #272
 ;; comp~ny hosts ~ web ~pplic~tion on ;;WS in the us-e~st-1  Region. The ~pplic~tion servers ~re distributed ~cross three ;;v~il~bility Zones behind ~n ;;pplic~tion  Lo~d  B~l~ncer. The d~t~b~se is hosted in ~  MySQL d~t~b~se on ~n ;;m~zon  EC2 inst~nce. ;; solutions ~rchitect needs to design ~ cross-Region d~t~ recovery solution using ;;WS services with ~n  RTO of less th~n 5 minutes ~nd ~n  RPO of less th~n  1 minute. The solutions ~rchitect is deploying ~pplic~tion servers in us-west-2, ~nd h~s con gured ;;m~zon  Route 53 he~lth checks ~nd  DNS f~ilover to us-west-2. Which ~ddition~l step should the solutions ~rchitect t~ke?
  ;;.  Migr~te the d~t~b~se to ~n ;;m~zon  RDS for  MySQL inst~nce with ~ cross-Region re~d replic~ in us-west-2.
  B.  Migr~te the d~t~b~se to ~n ;;m~zon ;;uror~ glob~l d~t~b~se with the prim~ry in us-e~st-1 ~nd the second~ry in us-west-2.
  C.  Migr~te the d~t~b~se to ~n ;;m~zon  RDS for  MySQL inst~nce with ~  Multi-;;Z deployment.
  D. Cre~te ~  MySQL st~ndby d~t~b~se on ~n ;;m~zon  EC2 inst~nce in us-west-2.

 Correct ;;nswer: D
 B (94%)                                    6%

 Question #273
 ;; comp~ny is using ;;WS Org~niz~tions to m~n~ge multiple ~ccounts.  Due to regul~tory requirements, the comp~ny w~nts to restrict speci c member ~ccounts to cert~in ;;WS  Regions, where they ~re permitted to deploy resources. The resources in the ~ccounts must be t~gged, enforced b~sed on ~ group st~nd~rd, ~nd centr~lly m~n~ged with minim~l con gur~tion. Wh~t should ~ solutions ~rchitect do to meet these requirements?
  ;;. Cre~te ~n ;;WS Con g rule in the speci c member ~ccounts to limit  Regions ~nd ~pply ~ t~g policy.
  B.  From the ;;WS  Billing ~nd Cost  M~n~gement console, in the m~n~gement ~ccount, dis~ble  Regions for the speci c member ~ccounts ~nd ~pply ~ t~g policy on the root.
  C. ;;ssoci~te the speci c member ~ccounts with the root. ;;pply ~ t~g policy ~nd ~n SCP using conditions to limit  Regions.
  D. ;;ssoci~te the speci c member ~ccounts with ~ new OU. ;;pply ~ t~g policy ~nd ~n SCP using conditions to limit  Regions.

 Correct ;;nswer: ;;
 D (100%)

 Question #274
 ;; comp~ny h~s ~n ~pplic~tion th~t gener~tes reports ~nd stores them in ~n ;;m~zon S3 bucket. When ~ user ~ccesses their report, the ~pplic~tion gener~tes ~ signed URL to ~llow the user to downlo~d the report. The comp~ny's security te~m h~s discovered th~t the  les ~re public ~nd th~t ~nyone c~n downlo~d them without ~uthentic~tion. The comp~ny h~s suspended the gener~tion of new reports until the problem is resolved. Which set of ~ctions will immedi~tely remedi~te the security issue without imp~cting the ~pplic~tion's norm~l work ow?
  ;;. Cre~te ~n ;;WS  L~mbd~ function th~t ~pplies ~ deny ~ll policy for users who ~re not ~uthentic~ted. Cre~te ~ scheduled event to invoke the L~mbd~ function.
  B.  Review the ;;WS Trusted ;;dvisor bucket permissions check ~nd implement the recommended ~ctions.
  C.  Run ~ script th~t puts ~ priv~te ;;CL on ~ll of the objects in the bucket.
  D. Use the  Block  Public ;;ccess fe~ture in ;;m~zon S3 to set the  IgnorePublic;;cIs option to TRUE on the bucket.

 Correct ;;nswer: B
 D (80%)                                  C (20%)

 Question #275
 ;; comp~ny is pl~nning to migr~te ~n ;;m~zon  RDS for Or~cle d~t~b~se to ~n  RDS for  PostgreSQL  DB inst~nce in ~nother ;;WS ~ccount. ;; solutions ~rchitect needs to design ~ migr~tion str~tegy th~t will require no downtime ~nd th~t will minimize the ~mount of time necess~ry to complete the migr~tion. The migr~tion str~tegy must replic~te ~ll existing d~t~ ~nd ~ny new d~t~ th~t is cre~ted during the migr~tion. The t~rget d~t~b~se must be identic~l to the source d~t~b~se ~t completion of the migr~tion process. ;;ll ~pplic~tions currently use ~n ;;m~zon  Route 53 CN;;ME record ~s their endpoint for communic~tion with the  RDS for Or~cle  DB inst~nce. The RDS for Or~cle  DB inst~nce is in ~ priv~te subnet. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose three.)
  ;;. Cre~te ~ new  RDS for  PostgreSQL  DB inst~nce in the t~rget ~ccount. Use the ;;WS Schem~ Conversion Tool (;;WS SCT) to migr~te the d~t~b~se schem~ from the source d~t~b~se to the t~rget d~t~b~se.
  B. Use the ;;WS Schem~ Conversion Tool (;;WS SCT) to cre~te ~ new  RDS for  PostgreSQL  DB inst~nce in the t~rget ~ccount with the schem~ ~nd initi~l d~t~ from the source d~t~b~se.
  C. Con gure VPC peering between the VPCs in the two ;;WS ~ccounts to provide connectivity to both  DB inst~nces from the t~rget ~ccount. Con gure the security groups th~t ~re ~tt~ched to e~ch  DB inst~nce to ~llow tr~ c on the d~t~b~se port from the VPC in the t~rget ~ccount.
  D. Tempor~rily ~llow the source  DB inst~nce to be publicly ~ccessible to provide connectivity from the VPC in the t~rget ~ccount. Con gure the security groups th~t ~re ~tt~ched to e~ch  DB inst~nce to ~llow tr~ c on the d~t~b~se port from the VPC in the t~rget ~ccount.
  E. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) in the t~rget ~ccount to perform ~ full lo~d plus ch~nge d~t~ c~pture (CDC) migr~tion from the source d~t~b~se to the t~rget d~t~b~se. When the migr~tion is complete, ch~nge the CN;;ME record to point to the t~rget  DB inst~nce endpoint.
  F. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) in the t~rget ~ccount to perform ~ ch~nge d~t~ c~pture (CDC) migr~tion from the source d~t~b~se to the t~rget d~t~b~se. When the migr~tion is complete, ch~nge the CN;;ME record to point to the t~rget  DB inst~nce endpoint.

 Correct ;;nswer: CEF
 ;;CE (96%)                                   4%

 Question #276
 ;; comp~ny h~s implemented ~n ordering system using ~n event-driven ~rchitecture.  During initi~l testing, the system stopped processing orders. Further log ~n~lysis reve~led th~t one order mess~ge in ~n ;;m~zon Simple Queue Service (;;m~zon SQS) st~nd~rd queue w~s c~using ~n error on the b~ckend ~nd blocking ~ll subsequent order mess~ges. The visibility timeout of the queue is set to 30 seconds, ~nd the b~ckend processing timeout is set to  10 seconds. ;; solutions ~rchitect needs to ~n~lyze f~ulty order mess~ges ~nd ensure th~t the system continues to process subsequent mess~ges. Which step should the solutions ~rchitect t~ke to meet these requirements?
  ;;.  Incre~se the b~ckend processing timeout to 30 seconds to m~tch the visibility timeout.
  B.  Reduce the visibility timeout of the queue to ~utom~tic~lly remove the f~ulty mess~ge.
  C. Con gure ~ new SQS  FIFO queue ~s ~ de~d-letter queue to isol~te the f~ulty mess~ges.
  D. Con gure ~ new SQS st~nd~rd queue ~s ~ de~d-letter queue to isol~te the f~ulty mess~ges.

 Correct ;;nswer: C
 D (82%)                                  C (18%)

 Question #277
 ;; comp~ny h~s ~utom~ted the nightly retr~ining of its m~chine le~rning models by using ;;WS Step  Functions. The work ow consists of multiple steps th~t use ;;WS  L~mbd~.  E~ch step c~n f~il for v~rious re~sons, ~nd ~ny f~ilure c~uses ~ f~ilure of the over~ll work ow. ;; review reve~ls th~t the retr~ining h~s f~iled multiple nights in ~ row without the comp~ny noticing the f~ilure. ;; solutions ~rchitect needs to improve the work ow so th~t noti c~tions ~re sent for ~ll types of f~ilures in the retr~ining process. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose three.)
  ;;. Cre~te ~n ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) topic with ~ subscription of type "Em~il" th~t t~rgets the te~m's m~iling list.
  B. Cre~te ~ t~sk n~med "Em~il" th~t forw~rds the input ~rguments to the SNS topic.
  C. ;;dd ~ C~tch  eld to ~ll T~sk,  M~p, ~nd  P~r~llel st~tes th~t h~ve ~ st~tement of "ErrorEqu~ls": [ "St~tes.;;LL" ] ~nd "Next”: "Em~il".
  D. ;;dd ~ new em~il ~ddress to ;;m~zon Simple  Em~il Service (;;m~zon SES). Verify the em~il ~ddress.
  E. Cre~te ~ t~sk n~med "Em~il" th~t forw~rds the input ~rguments to the SES em~il ~ddress.
  F. ;;dd ~ C~tch  eld to ~ll T~sk,  M~p, ~nd  P~r~llel st~tes th~t h~ve ~ st~tement of "ErrorEqu~ls": [ "St~tes.Runtime" ] ~nd "Next": "Em~il".

 Correct ;;nswer: BDE
 ;;BC (88%)                                    6%

 Question #278
 ;; comp~ny pl~ns to deploy ~ new priv~te intr~net service on ;;m~zon  EC2 inst~nces inside ~ VPC. ;;n ;;WS Site-to-Site VPN connects the VPC to the comp~ny's on-premises network. The new service must communic~te with existing on-premises services. The on-premises services ~re ~ccessible through the use of hostn~mes th~t reside in the comp~ny.ex~mple  DNS zone. This  DNS zone is wholly hosted on premises ~nd is ~v~il~ble only on the comp~ny's priv~te network. ;; solutions ~rchitect must ensure th~t the new service c~n resolve hostn~mes on the comp~ny.ex~mple dom~in to integr~te with existing services. Which solution meets these requirements?
  ;;. Cre~te ~n empty priv~te zone in ;;m~zon  Route 53 for comp~ny.ex~mple. ;;dd ~n ~ddition~l  NS record to the comp~ny's on-premises comp~ny.ex~mple zone th~t points to the ~uthorit~tive n~me servers for the new priv~te zone in  Route 53.
  B. Turn on  DNS hostn~mes for the VPC. Con gure ~ new outbound endpoint with ;;m~zon  Route 53  Resolver. Cre~te ~  Resolver rule to forw~rd requests for comp~ny.ex~mple to the on-premises n~me servers.
  C. Turn on  DNS hostn~mes for the VPCon gure ~ new inbound resolver endpoint with ;;m~zon  Route 53  Resolver. Con gur&the on-premises DNS server to forw~rd requests for comp~ny.ex~mple to the new resolver.
  D. Use ;;WS Systems  M~n~ger to con gure ~ run document th~t will inst~ll ~ hosts  le th~t cont~ins ~ny required hostn~mes. Use ~n ;;m~zon EventBridge rule to run the document when ~n inst~nce is entering the running st~te.

 Correct ;;nswer: ;;
 B (100%)

 Question #279
 ;; comp~ny uses ;;WS CloudForm~tion to deploy ~pplic~tions within multiple VPCs th~t ~re ~ll ~tt~ched to ~ tr~nsit g~tew~y.  E~ch VPC th~t sends tr~ c to the public internet must send the tr~ c through ~ sh~red services VPC.  E~ch subnet within ~ VPC uses the def~ult VPC route t~ble, ~nd the tr~ c is routed to the tr~nsit g~tew~y. The tr~nsit g~tew~y uses its def~ult route t~ble for ~ny VPC ~tt~chment. ;; security ~udit reve~ls th~t ~n ;;m~zon  EC2 inst~nce th~t is deployed within ~ VPC c~n communic~te with ~n  EC2 inst~nce th~t is deployed in ~ny of the comp~ny's other VPCs. ;; solutions ~rchitect needs to limit the tr~ c between the VPCs.  E~ch VPC must be ~ble to communic~te only with ~ prede ned, limited set of ~uthorized VPCs. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Upd~te the network ;;CL of e~ch subnet within ~ VPC to ~llow outbound tr~ c only to the ~uthorized VPCs.  Remove ~ll deny rules except the def~ult deny rule.
  B. Upd~te ~ll the security groups th~t ~re used within ~ VPC to deny outbound tr~ c to security groups th~t ~re used within the un~uthorized VPCs.
  C. Cre~te ~ dedic~ted tr~nsit g~tew~y route t~ble for e~ch VPC ~tt~chment.  Route tr~ c only to the ~uthorized VPCs.
  D. Upd~te the m~in route t~ble of e~ch VPC to route tr~ c only to the ~uthorized VPCs through the tr~nsit g~tew~y.

 Correct ;;nswer: C
 C (100%)

 Question #280
 ;; comp~ny h~s ~ Windows-b~sed desktop ~pplic~tion th~t is p~ck~ged ~nd deployed to the users' Windows m~chines. The comp~ny recently ~cquired ~nother comp~ny th~t h~s employees who prim~rily use m~chines with ~  Linux oper~ting system. The ~cquiring comp~ny h~s decided to migr~te ~nd rehost the Windows-b~sed desktop ~pplic~tion to ;;WS. ;;ll employees must be ~uthentic~ted before they use the ~pplic~tion. The ~cquiring comp~ny uses ;;ctive  Directory on premises but w~nts ~ simpli ed w~y to m~n~ge ~ccess to the ~pplic~tion on ;;WS for ~ll the employees. Which solution will rehost the ~pplic~tion on ;;WS with the  LE;;ST development effort?
  ;;. Set up ~nd provision ~n ;;m~zon Worksp~ces virtu~l desktop for every employee.  Implement ~uthentic~tion by using ;;m~zon Cognito identity pools.  Instruct employees to run the ~pplic~tion from their provisioned Worksp~ces virtu~l desktops.
  B. Cre~te ~n ;;uto Sc~ling group of Windows-b~sed ;;m~zon  EC2 inst~nces. Join e~ch  EC2 inst~nce to the comp~ny’s ;;ctive  Directory dom~in. Implement ~uthentic~tion by using the ;;ctive  Directory th~t is running on premises.  Instruct employees to run the ~pplic~tion by using ~ Windows remote desktop.
  C. Use ~n ;;m~zon ;;ppStre~m 2.0 im~ge builder to cre~te ~n im~ge th~t includes the ~pplic~tion ~nd the required con gur~tions.  Provision ~n ;;ppStre~m 2.0 On-Dem~nd  eet with dyn~mic  Fleet ;;uto Sc~ling policies for running the im~ge.  Implement ~uthentic~tion by using ;;ppStre~m 2.0 user pools.  Instruct the employees to ~ccess the ~pplic~tion by st~rting browser-b~sed ;;ppStre~m 2.0 stre~ming sessions.
  D.  Ref~ctor ~nd cont~inerize the ~pplic~tion to run ~s ~ web-b~sed ~pplic~tion.  Run the ~pplic~tion in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) on ;;WS  F~rg~te with step sc~ling policies.  Implement ~uthentic~tion by using ;;m~zon Cognito user pools.  Instruct the employees to run the ~pplic~tion from their browsers.

 Correct ;;nswer: D
 C (92%)                                    8%

 Question #281
 ;; comp~ny is collecting ~ l~rge ~mount of d~t~ from ~  eet of  IoT devices.  D~t~ is stored ~s Optimized  Row Column~r (ORC)  les in the  H~doop Distributed  File System (HDFS) on ~ persistent ;;m~zon  EMR cluster. The comp~ny's d~t~ ~n~lytics te~m queries the d~t~ by using SQL in ;;p~che Presto deployed on the s~me  EMR cluster. Queries sc~n l~rge ~mounts of d~t~, ~lw~ys run for less th~n  15 minutes, ~nd run only between 5  PM ~nd  10  PM. The comp~ny is concerned ~bout the high cost ~ssoci~ted with the current solution. ;; solutions ~rchitect must propose the most cost-effective solution th~t will ~llow SQL d~t~ queries. Which solution will meet these requirements?
  ;;. Store d~t~ in ;;m~zon S3. Use ;;m~zon  Redshift Spectrum to query d~t~.
  B. Store d~t~ in ;;m~zon S3. Use the ;;WS Glue  D~t~ C~t~log ~nd ;;m~zon ;;then~ to query d~t~.
  C. Store d~t~ in  EMR  File System (EMRFS). Use  Presto in ;;m~zon  EMR to query d~t~.
  D. Store d~t~ in ;;m~zon  Redshift. Use ;;m~zon  Redshift to query d~t~.

 Correct ;;nswer: D
 B (100%)

 Question #282
 ;; l~rge comp~ny recently experienced ~n unexpected incre~se in ;;m~zon  RDS ~nd ;;m~zon  Dyn~moDB costs. The comp~ny needs to incre~se visibility into det~ils of ;;WS  Billing ~nd Cost  M~n~gement. There ~re v~rious ~ccounts ~ssoci~ted with ;;WS Org~niz~tions, including m~ny development ~nd production ~ccounts. There is no consistent t~gging str~tegy ~cross the org~niz~tion, but there ~re guidelines in pl~ce th~t require ~ll infr~structure to be deployed using ;;WS CloudForm~tion with consistent t~gging.  M~n~gement requires cost center numbers ~nd project  ID numbers for ~ll existing ~nd future  Dyn~moDB t~bles ~nd  RDS inst~nces. Which str~tegy should the solutions ~rchitect provide to meet these requirements?
  ;;. Use T~g  Editor to t~g existing resources. Cre~te cost ~lloc~tion t~gs to de ne the cost center ~nd project  ID ~nd ~llow 24 hours for t~gs to prop~g~te to existing resources.
  B. Use ~n ;;WS Con g rule to ~lert the  n~nce te~m of unt~gged resources. Cre~te ~ centr~lized ;;WS  L~mbd~ b~sed solution to t~g unt~gged RDS d~t~b~ses ~nd  Dyn~moDB resources every hour using ~ cross-~ccount role.
  C. Use T~g  Editor to t~g existing resources. Cre~te cost ~lloc~tion t~gs to de ne the cost center ~nd project  ID. Use SCPs to restrict resource cre~tion th~t do not h~ve the cost center ~nd project  ID on the resource.
  D. Cre~te cost ~lloc~tion t~gs to de ne the cost center ~nd project  ID ~nd ~llow 24 hours for t~gs to prop~g~te to existing resources. Upd~te existing feder~ted roles to restrict privileges to provision resources th~t do not include the cost center ~nd project  ID on the resource.

 Correct ;;nswer: B
 C (86%)                                    14%

 Question #283
 ;; comp~ny w~nts to send d~t~ from its on-premises systems to ;;m~zon S3 buckets. The comp~ny cre~ted the S3 buckets in three different ~ccounts. The comp~ny must send the d~t~ priv~tely without the d~t~ tr~veling ~cross the internet. The comp~ny h~s no existing dedic~ted connectivity to ;;WS. Which combin~tion of steps should ~ solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;.  Est~blish ~ networking ~ccount in the ;;WS Cloud. Cre~te ~ priv~te VPC in the networking ~ccount. Set up ~n ;;WS  Direct Connect connection with ~ priv~te VIF between the on-premises environment ~nd the priv~te VPC.
  B.  Est~blish ~ networking ~ccount in the ;;WS Cloud. Cre~te ~ priv~te VPC in the networking ~ccount. Set up ~n ;;WS  Direct Connect connection with ~ public VIF between the on-premises environment ~nd the priv~te VPC.
  C. Cre~te ~n ;;m~zon S3 interf~ce endpoint in the networking ~ccount.
  D. Cre~te ~n ;;m~zon S3 g~tew~y endpoint in the networking ~ccount.
  E.  Est~blish ~ networking ~ccount in the ;;WS Cloud. Cre~te ~ priv~te VPC in the networking ~ccount.  Peer VPCs from the ~ccounts th~t host the S3 buckets with the VPC in the network ~ccount.

 Correct ;;nswer: D;;
 ;;C (73%)                             14%         9%

 Question #284
 ;; comp~ny oper~tes quick-service rest~ur~nts. The rest~ur~nts follow ~ predict~ble model with high s~les tr~ c for 4 hours d~ily. S~les tr~ c is lower outside of those pe~k hours. The point of s~le ~nd m~n~gement pl~tform is deployed in the ;;WS Cloud ~nd h~s ~ b~ckend th~t is b~sed on ;;m~zon  Dyn~moDB. The d~t~b~se t~ble uses provisioned throughput mode with  100,000  RCUs ~nd 80,000 WCUs to m~tch known pe~k resource consumption. The comp~ny w~nts to reduce its  Dyn~moDB cost ~nd minimize the oper~tion~l overhe~d for the  IT st~ff. Which solution meets these requirements  MOST cost-effectively?
  ;;.  Reduce the provisioned  RCUs ~nd WCUs.
  B. Ch~nge the  Dyn~moDB t~ble to use on-dem~nd c~p~city.
  C.  En~ble  Dyn~mo  DB ~uto sc~ling for the t~ble.
  D.  Purch~se  1-ye~r reserved c~p~city th~t is su cient to cover the pe~k lo~d for 4 hours e~ch d~y.

 Correct ;;nswer: ;;
 C (75%)                                  D (25%)

 Question #285
 ;; comp~ny hosts ~ blog post ~pplic~tion on ;;WS using ;;m~zon ;;PI G~tew~y, ;;m~zon  Dyn~moDB, ~nd ;;WS  L~mbd~. The ~pplic~tion currently does not use ;;PI keys to ~uthorize requests. The ;;PI model is ~s follows: GET /posts/{postId}: to get post det~ils GET /users/{userId}: to get user det~ils GET /comments/{commentId}: to get comments det~ils The comp~ny h~s noticed users ~re ~ctively discussing topics in the comments section, ~nd the comp~ny w~nts to incre~se user eng~gement by m~king the comments ~ppe~r in re~l time. Which design should be used to reduce comment l~tency ~nd improve user experience?
  ;;. Use edge-optimized ;;PI with ;;m~zon CloudFront to c~che ;;PI responses.
  B.  Modify the blog ~pplic~tion code to request GET/comments/{commentId} every  10 seconds.
  C. Use ;;WS ;;ppSync ~nd lever~ge WebSockets to deliver comments.
  D. Ch~nge the concurrency limit of the  L~mbd~ functions to lower the ;;PI response time.

 Correct ;;nswer: C
 C (100%)

 Question #286
 ;; comp~ny m~n~ges hundreds of ;;WS ~ccounts centr~lly in ~n org~niz~tion in ;;WS Org~niz~tions. The comp~ny recently st~rted to ~llow product te~ms to cre~te ~nd m~n~ge their own S3 ~ccess points in their ~ccounts. The S3 ~ccess points c~n be ~ccessed only within VPCs, not on the internet. Wh~t is the  MOST oper~tion~lly e cient w~y to enforce this requirement?
  ;;. Set the S3 ~ccess point resource policy to deny the s3:Cre~te;;ccessPoint ~ction unless the s3:;;ccessPointNetworkOrigin condition key ev~lu~tes to VPC.
  B. Cre~te ~n SCP ~t the root level in the org~niz~tion to deny the s3:Cre~te;;ccessPoint ~ction unless the s3:;;ccessPointNetworkOrigin condition key ev~lu~tes to VPC.
  C. Use ;;WS CloudForm~tion St~ckSets to cre~te ~ new  I;;M policy in e~ch ;;WS ~ccount th~t ~llows the s3:Cre~te;;ccessPoint ~ction only if the s3:;;ccessPointNetworkOrigin condition key ev~lu~tes to VPC.
  D. Set the S3 bucket policy to deny the s3:Cre~te;;ccessPoint ~ction unless the s3:;;ccessPointNetworkOrigin condition key ev~lu~tes to VPC.

 Correct ;;nswer: ;;
 B (93%)                                    7%

 Question #287
 ;; solutions ~rchitect must upd~te ~n ~pplic~tion environment within ;;WS  El~stic  Be~nst~lk using ~ blue/green deployment methodology. The solutions ~rchitect cre~tes ~n environment th~t is identic~l to the existing ~pplic~tion environment ~nd deploys the ~pplic~tion to the new environment. Wh~t should be done next to complete the upd~te?
  ;;.  Redirect to the new environment using ;;m~zon  Route 53.
  B. Select the Sw~p  Environment URLs option.
  C.  Repl~ce the ;;uto Sc~ling l~unch con gur~tion.
  D. Upd~te the  DNS records to point to the green environment.

 Correct ;;nswer: ;;
 B (100%)

 Question #288
 ;; comp~ny is building ~n im~ge service on the web th~t will ~llow users to uplo~d ~nd se~rch r~ndom photos. ;;t pe~k us~ge, up to  10,000 users worldwide will uplo~d their im~ges. The will then overl~y text on the uplo~ded im~ges, which will then be published on the comp~ny website. Which design should ~ solutions ~rchitect implement?
  ;;. Store the uplo~ded im~ges in ;;m~zon  El~stic  File System (;;m~zon  EFS). Send ~pplic~tion log inform~tion ~bout e~ch im~ge to ;;m~zon CloudW~tch  Logs. Cre~te ~  eet of ;;m~zon  EC2 inst~nces th~t use CloudW~tch  Logs to determine which im~ges need to be processed.  Pl~ce processed im~ges in ~nother directory in ;;m~zon  EFS.  En~ble ;;m~zon CloudFront ~nd con gure the origin to be the one of the  EC2 inst~nces in the  eet.
  B. Store the uplo~ded im~ges in ~n ;;m~zon S3 bucket ~nd con gure ~n S3 bucket event noti c~tion to send ~ mess~ge to ;;m~zon Simple Noti c~tion Service (;;m~zon SNS). Cre~te ~  eet of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) to pull mess~ges from ;;m~zon SNS to process the im~ges ~nd pl~ce them in ;;m~zon  El~stic  File System (;;m~zon  EFS). Use ;;m~zon CloudW~tch metrics for the SNS mess~ge volume to sc~le out  EC2 inst~nces.  En~ble ;;m~zon CloudFront ~nd con gure the origin to be the ;;LB in front of the  EC2 inst~nces.
  C. Store the uplo~ded im~ges in ~n ;;m~zon S3 bucket ~nd con gure ~n S3 bucket event noti c~tion to send ~ mess~ge to the ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Cre~te ~  eet of ;;m~zon  EC2 inst~nces to pull mess~ges from the SQS queue to process the im~ges ~nd pl~ce them in ~nother S3 bucket. Use ;;m~zon CloudW~tch metrics for queue depth to sc~le out  EC2 inst~nces.  En~ble ;;m~zon CloudFront ~nd con gure the origin to be the S3 bucket th~t cont~ins the processed im~ges.
  D. Store the uplo~ded im~ges on ~ sh~red ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume mounted to ~  eet of ;;m~zon  EC2 Spot inst~nces. Cre~te ~n ;;m~zon  Dyn~moDB t~ble th~t cont~ins inform~tion ~bout e~ch uplo~ded im~ge ~nd whether it h~s been processed. Use ~n ;;m~zon  EventBridge rule to sc~le out  EC2 inst~nces.  En~ble ;;m~zon CloudFront ~nd con gure the origin to reference ~n  El~stic  Lo~d B~l~ncer in front of the  eet of  EC2 inst~nces.

 Correct ;;nswer: D
 C (100%)

 Question #289
 ;; comp~ny h~s deployed its d~t~b~se on ~n ;;m~zon  RDS for  MySQL  DB inst~nce in the us-e~st-1  Region. The comp~ny needs to m~ke its d~t~ ~v~il~ble to customers in  Europe. The customers in  Europe must h~ve ~ccess to the s~me d~t~ ~s customers in the United St~tes (US) ~nd will not toler~te high ~pplic~tion l~tency or st~le d~t~. The customers in  Europe ~nd the customers in the US need to write to the d~t~b~se.  Both groups of customers need to see upd~tes from the other group in re~l time. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;m~zon ;;uror~  MySQL replic~ of the  RDS for  MySQL  DB inst~nce.  P~use ~pplic~tion writes to the  RDS  DB inst~nce.  Promote the ;;uror~  Replic~ to ~ st~nd~lone  DB cluster.  Recon gure the ~pplic~tion to use the ;;uror~ d~t~b~se ~nd resume writes. ;;dd eu-west-1 ~s ~ second~ry  Region to the  DB cluster.  En~ble write forw~rding on the  DB cluster.  Deploy the ~pplic~tion in eu-west-1. Con gure the ~pplic~tion to use the ;;uror~  MySQL endpoint in eu-west-1.
  B. ;;dd ~ cross-Region replic~ in eu-west-1 for the  RDS for  MySQL  DB inst~nce. Con gure the replic~ to replic~te write queries b~ck to the prim~ry  DB inst~nce.  Deploy the ~pplic~tion in eu-west-1. Con gure the ~pplic~tion to use the  RDS for  MySQL endpoint in eu-west-1.
  C. Copy the most recent sn~pshot from the  RDS for  MySQL  DB inst~nce to eu-west-1. Cre~te ~ new  RDS for  MySQL  DB inst~nce in eu-west-1 from the sn~pshot. Con gure  MySQL logic~l replic~tion from us-e~st-1 to eu-west-1.  En~ble write forw~rding on the  DB cluster.  Deploy the ~pplic~tion in eu-wes&1. Con gure the ~pplic~tion to use the  RDS for  MySQL endpoint in eu-west-1.
  D. Convert the  RDS for  MySQL  DB inst~nce to ~n ;;m~zon ;;uror~  MySQL  DB cluster. ;;dd eu-west-1 ~s ~ second~ry  Region to the  DB cluster. En~ble write forw~rding on the  DB cluster.  Deploy the ~pplic~tion in eu-west-1. Con gure the ~pplic~tion to use the ;;uror~  MySQL endpoint in eu-west-1.

 Correct ;;nswer: B
 ;; (62%)                                  D (38%)

 Question #290
 ;; comp~ny is serving  les to its customers through ~n SFTP server th~t is ~ccessible over the internet. The SFTP server is running on ~ single ;;m~zon  EC2 inst~nce with ~n  El~stic  IP ~ddress ~tt~ched. Customers connect to the SFTP server through its  El~stic  IP ~ddress ~nd use SSH for ~uthentic~tion. The  EC2 inst~nce ~lso h~s ~n ~tt~ched security group th~t ~llows ~ccess from ~ll customer  IP ~ddresses. ;; solutions ~rchitect must implement ~ solution to improve ~v~il~bility, minimize the complexity of infr~structure m~n~gement, ~nd minimize the disruption to customers who ~ccess  les. The solution must not ch~nge the w~y customers connect. Which solution will meet these requirements?
  ;;.  Dis~ssoci~te the  El~stic  IP ~ddress from the  EC2 inst~nce. Cre~te ~n ;;m~zon S3 bucket to be used for SFTP  le hosting. Cre~te ~n ;;WS Tr~nsfer  F~mily server. Con gure the Tr~nsfer  F~mily server with ~ publicly ~ccessible endpoint. ;;ssoci~te the SFTP  El~stic  IP ~ddress with the new endpoint.  Point the Tr~nsfer  F~mily server to the S3 bucket. Sync ~ll  les from the SFTP server to the S3 bucket.
  B.  Dis~ssoci~te the  El~stic  IP ~ddress from the  EC2 inst~nce. Cre~te ~n ;;m~zon S3 bucket to be used for SFTP  le hosting. Cre~te ~n ;;WS Tr~nsfer  F~mily server. Con gure the Tr~nsfer  F~mily server with ~ VPC-hosted, internet-f~cing endpoint. ;;ssoci~te the SFTP  El~stic  IP ~ddress with the new endpoint. ;;tt~ch the security group with customer  IP ~ddresses to the new endpoint.  Point the Tr~nsfer  F~mily server to the S3 bucket. Sync ~ll  les from the SFTP server to the S3 bucket.
  C.  Dis~ssoci~te the  El~stic  IP ~ddress from the  EC2 inst~nce. Cre~te ~ new ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system to be used for SFTP  le hosting. Cre~te ~n ;;WS  F~rg~te t~sk de nition to run ~n SFTP server. Specify the  EFS  le system ~s ~ mount in the t~sk de nition. Cre~te ~  F~rg~te service by using the t~sk de nition, ~nd pl~ce ~  Network  Lo~d  B~l~ncer (NLB) in front of the service. When con guring the service, ~tt~ch the security group with customer  IP ~ddresses to the t~sks th~t run the SFTP server. ;;ssoci~te the  El~stic  IP ~ddress with the  NLB. Sync ~ll  les from the SFTP server to the S3 bucket.
  D.  Dis~ssoci~te the  El~stic  IP ~ddress from the  EC2 inst~nce. Cre~te ~ multi-~tt~ch ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume to be used for SFTP  le hosting. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) with the  El~stic  IP ~ddress ~tt~ched. Cre~te ~n ;;uto Sc~ling group with  EC2 inst~nces th~t run ~n SFTP server.  De ne in the ;;uto Sc~ling group th~t inst~nces th~t ~re l~unched should ~tt~ch the new multi-~tt~ch  EBS volume. Con gure the ;;uto Sc~ling group to ~utom~tic~lly ~dd inst~nces behind the  NLB. Con gure the ;;uto Sc~ling group to use the security group th~t ~llows customer  IP ~ddresses for the  EC2 inst~nces th~t the ;;uto Sc~ling group l~unches. Sync ~ll  les from the SFTP server to the new multi-~tt~ch  EBS volume.

 Correct ;;nswer: C
 B (89%)                                    11%

 Question #291
 ;; comp~ny ingests ~nd processes stre~ming m~rket d~t~. The d~t~ r~te is const~nt. ;; nightly process th~t c~lcul~tes ~ggreg~te st~tistics t~kes 4 hours to complete. The st~tistic~l ~n~lysis is not critic~l to the business, ~nd d~t~ points ~re processed during the next iter~tion if ~ p~rticul~r run f~ils. The current ~rchitecture uses ~ pool of ;;m~zon  EC2  Reserved  Inst~nces with  1-ye~r reserv~tions. These  EC2 inst~nces run full time to ingest ~nd store the stre~ming d~t~ in ~tt~ched ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes. ;; scheduled script l~unches  EC2 On-Dem~nd  Inst~nces e~ch night to perform the nightly processing. The inst~nces ~ccess the stored d~t~ from  NFS sh~res on the ingestion servers. The script termin~tes the inst~nces when the processing is complete. The  Reserved  Inst~nce reserv~tions ~re expiring. The comp~ny needs to determine whether to purch~se new reserv~tions or implement ~ new design. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Upd~te the ingestion process to use ;;m~zon  Kinesis  D~t~  Firehose to s~ve d~t~ to ;;m~zon S3. Use ~ scheduled script to l~unch ~  eet of EC2 On-Dem~nd  Inst~nces e~ch night to perform the b~tch processing of the S3 d~t~. Con gure the script to termin~te the inst~nces when the processing is complete.
  B. Upd~te the ingestion process to use ;;m~zon  Kinesis  D~t~  Firehose to s~ve d~t~ to ;;m~zon S3. Use ;;WS  B~tch with Spot  Inst~nces to perform nightly processing with ~ m~ximum Spot price th~t is 50% of the On-Dem~nd price.
  C. Upd~te the ingestion process to use ~  eet of  EC2  Reserved  Inst~nces with 3-ye~r reserv~tions behind ~  Network  Lo~dB~l~ncer. Use ;;WS B~tch with Spot  Inst~nces to perform nightly processing with ~ m~ximum Spot price th~t is 50% of the On-Dem~nd price.
  D. Upd~te the ingestion process to use ;;m~zon  Kinesis  D~t~  Firehose to s~ve d~t~ to ;;m~zon  Redshift. Use ;;m~zon  EventBridge to schedule ~n ;;WS  L~mbd~ function to run nightly to query ;;m~zon  Redshift to gener~te the d~ily st~tistics.

 Correct ;;nswer: ;;
 B (93%)                                     7%

 Question #292
 ;; comp~ny needs to migr~te ~n on-premises SFTP site to ;;WS. The SFTP site currently runs on ~  Linux VM. Uplo~ded  les ~re m~de ~v~il~ble to downstre~m ~pplic~tions through ~n  NFS sh~re. ;;s p~rt of the migr~tion to ;;WS, ~ solutions ~rchitect must implement high ~v~il~bility. The solution must provide extern~l vendors with ~ set of st~tic public  IP ~ddresses th~t the vendors c~n ~llow. The comp~ny h~s set up ~n ;;WS  Direct Connect connection between its on-premises d~t~ center ~nd its VPC. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n ;;WS Tr~nsfer  F~mily server. Con gure ~n internet-f~cing VPC endpoint for the Tr~nsfer  F~mily server. Specify ~n  El~stic  IP ~ddress for e~ch subnet. Con gure the Tr~nsfer  F~mily server to pl~ce  les into ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system th~t is deployed ~cross multiple ;;v~il~bility Zones.  Modify the con gur~tion on the downstre~m ~pplic~tions th~t ~ccess the existing  NFS sh~re to mount the  EFS endpoint inste~d.
  B. Cre~te ~n ;;WS Tr~nsfer  F~mily server. Con gure ~ publicly ~ccessible endpoint for the Tr~nsfer  F~mily server. Con gure the Tr~nsfer  F~mily server to pl~ce  les into ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system th~t is deployed ~cross multiple ;;v~il~bility Zones.  Modify the con gur~tion on the downstre~m ~pplic~tions th~t ~ccess the existing  NFS sh~re to mount the  EFS endpoint inste~d.
  C. Use ;;WS ;;pplic~tion  Migr~tion Service to migr~te the existing  Linux VM to ~n ;;m~zon  EC2 inst~nce. ;;ssign ~n  El~stic  IP ~ddress to the EC2 inst~nce.  Mount ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system to the  EC2 inst~nce. Con gure the SFTP server to pl~ce  les in the  EFS  le system.  Modify the con gur~tion on the downstre~m ~pplic~tions th~t ~ccess the existing  NFS sh~re to mount the  EFS endpoint inste~d.
  D. Use ;;WS ;;pplic~tion  Migr~tion Service to migr~te the existing  Linux VM to ~n ;;WS Tr~nsfer  F~mily server. Con gure ~ publicly ~ccessible endpoint for the Tr~nsfer  F~mily server. Con gure the Tr~nsfer  F~mily server to pl~ce  les into ~n ;;m~zon  FSx for  Lustre  le system th~t is deployed ~cross multiple ;;v~il~bility Zones.  Modify the con gur~tion on the downstre~m ~pplic~tions th~t ~ccess the existing  NFS sh~re to mount the  FSx for  Lustre endpoint inste~d.

 Correct ;;nswer: B
 ;; (100%)

 Question #293
 ;; solutions ~rchitect h~s ~n oper~tion~l worklo~d deployed on ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group. The VPC ~rchitecture sp~ns two ;;v~il~bility Zones (;;Z) with ~ subnet in e~ch th~t the ;;uto Sc~ling group is t~rgeting. The VPC is connected to ~n on-premises environment ~nd connectivity c~nnot be interrupted. The m~ximum size of the ;;uto Sc~ling group is 20 inst~nces in service. The VPC  IPv4 ~ddressing is ~s follows: VPC CIDR:  10.0.0.0/23 - ;;Z1 subnet CIDR:  10.0.0.0/24 - ;;Z2 subnet CIDR:  10.0.1.0/24 - Since deployment, ~ third ;;Z h~s become ~v~il~ble in the  Region. The solutions ~rchitect w~nts to ~dopt the new ;;Z without ~dding ~ddition~l IPv4 ~ddress sp~ce ~nd without service downtime. Which solution will meet these requirements?
  ;;. Upd~te the ;;uto Sc~ling group to use the ;;Z2 subnet only.  Delete ~nd re-cre~te the ;;Z1 subnet using h~lf the previous ~ddress sp~ce. ;;djust the ;;uto Sc~ling group to ~lso use the new ;;Z1 subnet. When the inst~nces ~re he~lthy, ~djust the ;;uto Sc~ling group to use the ;;Z1 subnet only.  Remove the current ;;Z2 subnet. Cre~te ~ new ;;Z2 subnet using the second h~lf of the ~ddress sp~ce from the origin~l ;;Z1 subnet. Cre~te ~ new ;;Z3 subnet using h~lf the origin~l ;;Z2 subnet ~ddress sp~ce, then upd~te the ;;uto Sc~ling group to t~rget ~ll three new subnets.
  B. Termin~te the  EC2 inst~nces in the ;;Z1 subnet.  Delete ~nd re-cre~te the ;;Z1 subnet using h~lf the ~ddress sp~ce. Upd~te the ;;uto Sc~ling group to use this new subnet.  Repe~t this for the second ;;Z.  De ne ~ new subnet in ;;Z3, then upd~te the ;;uto Sc~ling group to t~rget ~ll three new subnets.
  C. Cre~te ~ new VPC with the s~me  IPv4 ~ddress sp~ce ~nd de ne three subnets, with one for e~ch ;;Z. Upd~te the existing ;;uto Sc~ling group to t~rget the new subnets in the new VPC.
  D. Upd~te the ;;uto Sc~ling group to use the ;;Z2 subnet only. Upd~te the ;;Z1 subnet to h~ve h~lf the previous ~ddress sp~ce. ;;djust the ;;uto Sc~ling group to ~lso use the ;;Z1 subnet ~g~in. When the inst~nces ~re he~lthy, ~djust the ;;uto Sc~ling group to use the ;;Z1 subnet only. Upd~te the current ;;Z2 subnet ~nd ~ssign the second h~lf of the ~ddress sp~ce from the origin~l ;;Z1 subnet. Cre~te ~ new ;;Z3 subnet using h~lf the origin~l ;;Z2 subnet ~ddress sp~ce, then upd~te the ;;uto Sc~ling group to t~rget ~ll three new subnets.

 Correct ;;nswer: D
 ;; (87%)                                   13%

 Question #294
 ;; comp~ny uses ~n org~niz~tion in ;;WS Org~niz~tions to m~n~ge the comp~ny's ;;WS ~ccounts. The comp~ny uses ;;WS CloudForm~tion to deploy ~ll infr~structure. ;;  n~nce te~m w~nts to build ~ ch~rgeb~ck model. The  n~nce te~m ~sked e~ch business unit to t~g resources by using ~ prede ned list of project v~lues. When the  n~nce te~m used the ;;WS Cost ~nd Us~ge  Report in ;;WS Cost  Explorer ~nd  ltered b~sed on project, the te~m noticed noncompli~nt project v~lues. The comp~ny w~nts to enforce the use of project t~gs for new resources. Which solution will meet these requirements with the  LE;;ST effort?
  ;;. Cre~te ~ t~g policy th~t cont~ins the ~llowed project t~g v~lues in the org~niz~tion's m~n~gement ~ccount. Cre~te ~n SCP th~t denies the cloudform~tion:Cre~teSt~ck ;;PI oper~tion unless ~ project t~g is ~dded. ;;tt~ch the SCP to e~ch OU.
  B. Cre~te ~ t~g policy th~t cont~ins the ~llowed project t~g v~lues in e~ch OU. Cre~te ~n SCP th~t denies the cloudform~tion:Cre~teSt~ck ;;PI oper~tion unless ~ project t~g is ~dded. ;;tt~ch the SCP to e~ch OU.
  C. Cre~te ~ t~g policy th~t cont~ins the ~llowed project t~g v~lues in the ;;WS m~n~gement ~ccount. Cre~te ~n  I;;M policy th~t denies the cloudform~tion:Cre~teSt~ck ;;PI oper~tion unless ~ project t~g is ~dded. ;;ssign the policy to e~ch user.
  D. Use ;;WS Service C~t~log to m~n~ge the CloudForm~tion st~cks ~s products. Use ~ T~gOptions libr~ry to control project t~g v~lues. Sh~re the portfolio with ~ll OUs th~t ~re in the org~niz~tion.

 Correct ;;nswer: C
 ;; (100%)

 Question #295
 ;;n ~pplic~tion is deployed on ;;m~zon  EC2 inst~nces th~t run in ~n ;;uto Sc~ling group. The ;;uto Sc~ling group con gur~tion uses only one type of inst~nce. CPU ~nd memory utiliz~tion metrics show th~t the inst~nces ~re underutilized. ;; solutions ~rchitect needs to implement ~ solution to perm~nently reduce the  EC2 cost ~nd incre~se the utiliz~tion. Which solution will meet these requirements with the  LE;;ST number of con gur~tion ch~nges in the future?
  ;;.  List inst~nce types th~t h~ve properties th~t ~re simil~r to the properties th~t the current inst~nces h~ve.  Modify the ;;uto Sc~ling group's l~unch templ~te con gur~tion to use multiple inst~nce types from the list.
  B. Use the inform~tion ~bout the ~pplic~tion's CPU ~nd memory utiliz~tion to select ~n inst~nce type th~t m~tches the requirements.  Modify the ;;uto Sc~ling group's con gur~tion by ~dding the new inst~nce type.  Remove the current inst~nce type from the con gur~tion.
  C. Use the inform~tion ~bout the ~pplic~tion's CPU ~nd memory utiliz~tion to specify CPU ~nd memory requirements in ~ new revision of the ;;uto Sc~ling group's l~unch templ~te.  Remove the current inst~nce type from the con gur~tion.
  D. Cre~te ~ script th~t selects the ~ppropri~te inst~nce types from the ;;WS  Price  List  Bulk ;;PI. Use the selected inst~nce types to cre~te ~ new revision of the ;;uto Sc~ling group's l~unch templ~te.

 Correct ;;nswer: B
 C (70%)                                  B (30%)

 Question #296
 ;; comp~ny implements ~ cont~inerized ~pplic~tion by using ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) ~nd ;;m~zon ;;PI G~tew~y The ~pplic~tion d~t~ is stored in ;;m~zon ;;uror~ d~t~b~ses ~nd ;;m~zon  Dyn~moDB d~t~b~ses. The comp~ny ~utom~tes infr~structure provisioning by using ;;WS CloudForm~tion. The comp~ny ~utom~tes ~pplic~tion deployment by using ;;WS CodePipeline. ;; solutions ~rchitect needs to implement ~ dis~ster recovery (DR) str~tegy th~t meets ~n  RPO of 2 hours ~nd ~n  RTO of 4 hours. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Set up ~n ;;uror~ glob~l d~t~b~se ~nd  Dyn~moDB glob~l t~bles to replic~te the d~t~b~ses to ~ second~ry ;;WS  Region.  In the prim~ry Region ~nd in the second~ry  Region, con gure ~n ;;PI G~tew~y ;;PI with ~  Region~l endpoint.  Implement ;;m~zon CloudFront with origin f~ilover to route tr~ c to the second~ry  Region during ~  DR scen~rio.
  B. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS), ;;m~zon  EventBridge, ~nd ;;WS  L~mbd~ to replic~te the ;;uror~ d~t~b~ses to ~ second~ry ;;WS  Region. Use  Dyn~moDB Stre~ms,  EventBridge. ~nd  L~mbd~ to replic~te the  Dyn~moDB d~t~b~ses to the second~ry  Region.  In the prim~ry  Region ~nd in the second~ry  Region, con gure ~n ;;PI G~tew~y ;;PI with ~  Region~l endpoint.  Implement ;;m~zon  Route 53 f~ilover routing to switch tr~ c from the prim~ry  Region to the second~ry  Region.
  C. Use ;;WS  B~ckup to cre~te b~ckups of the ;;uror~ d~t~b~ses ~nd the  Dyn~moDB d~t~b~ses in ~ second~ry ;;WS  Region.  In the prim~ry Region ~nd in the second~ry  Region, con gure ~n ;;PI G~tew~y ;;PI with ~  Region~l endpoint.  Implement ;;m~zon  Route 53 f~ilover routing to switch tr~ c from the prim~ry  Region to the second~ry  Region.
  D. Set up ~n ;;uror~ glob~l d~t~b~se ~nd  Dyn~moDB glob~l t~bles to replic~te the d~t~b~ses to ~ second~ry ;;WS  Region.  In the prim~ry Region ~nd in the second~ry  Region, con gure ~n ;;PI G~tew~y ;;PI with ~  Region~l endpoint.  Implement ;;m~zon  Route 53 f~ilover routing to switch tr~ c from the prim~ry  Region to the second~ry  Region.

 Correct ;;nswer: ;;
 C (63%)                                D (32%)          5%

 Question #297
 ;; comp~ny h~s ~ complex web ~pplic~tion th~t lever~ges ;;m~zon CloudFront for glob~l sc~l~bility ~nd perform~nce. Over time, users report th~t the web ~pplic~tion is slowing down. The comp~ny's oper~tions te~m reports th~t the CloudFront c~che hit r~tio h~s been dropping ste~dily. The c~che metrics report indic~tes th~t query strings on some URLs ~re inconsistently ordered ~nd ~re speci ed sometimes in mixed-c~se letters ~nd sometimes in lowerc~se letters. Which set of ~ctions should the solutions ~rchitect t~ke to incre~se the c~che hit r~tio ~s quickly ~s possible?
  ;;.  Deploy ~  L~mbd~@Edge function to sort p~r~meters by n~me ~nd force them to be lowerc~se. Select the CloudFront viewer request trigger to invoke the function.
  B. Upd~te the CloudFront distribution to dis~ble c~ching b~sed on query string p~r~meters.
  C.  Deploy ~ reverse proxy ~fter the lo~d b~l~ncer to post-process the emitted URLs in the ~pplic~tion to force the URL strings to be lowerc~se.
  D. Upd~te the CloudFront distribution to specify c~sing-insensitive query string processing.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #298
 ;; comp~ny runs ~n ecommerce ~pplic~tion in ~ single ;;WS  Region. The ~pplic~tion uses ~  ve-node ;;m~zon ;;uror~  MySQL  DB cluster to store inform~tion ~bout customers ~nd their recent orders. The  DB cluster experiences ~ l~rge number of write tr~ns~ctions throughout the d~y. The comp~ny needs to replic~te the d~t~ in the ;;uror~ d~t~b~se to ~nother  Region to meet dis~ster recovery requirements. The comp~ny h~s ~n RPO of  1 hour. Which solution will meet these requirements with the  LOWEST cost?
  ;;.  Modify the ;;uror~ d~t~b~se to be ~n ;;uror~ glob~l d~t~b~se. Cre~te ~ second ;;uror~ d~t~b~se in ~nother  Region.
  B.  En~ble the  B~cktr~ck fe~ture for the ;;uror~ d~t~b~se. Cre~te ~n ;;WS  L~mbd~ function th~t runs d~ily to copy the sn~pshots of the d~t~b~se to ~ b~ckup  Region.
  C. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS). Cre~te ~  DMS ch~nge d~t~ c~pture (CDC) t~sk th~t replic~tes the ongoing ch~nges from the ;;uror~ d~t~b~se to ~n ;;m~zon S3 bucket in ~nother  Region.
  D. Turn off ~utom~ted ;;uror~ b~ckups. Con gure ;;uror~ b~ckups with ~ b~ckup frequency of  1 hour. Specify ~nother  Region ~s the destin~tion  Region. Select the ;;uror~ d~t~b~se ~s the resource ~ssignment.

 Correct ;;nswer: C
 C (80%)                                  ;; (20%)

 Question #299
 ;; comp~ny's solutions ~rchitect is ev~lu~ting ~n ;;WS worklo~d th~t w~s deployed sever~l ye~rs ~go. The ~pplic~tion tier is st~teless ~nd runs on ~ single l~rge ;;m~zon  EC2 inst~nce th~t w~s l~unched from ~n ;;MI. The ~pplic~tion stores d~t~ in ~  MySQL d~t~b~se th~t runs on ~ single  EC2 inst~nce. The CPU utiliz~tion on the ~pplic~tion server  EC2 inst~nce often re~ches  100% ~nd c~uses the ~pplic~tion to stop responding. The comp~ny m~nu~lly inst~lls p~tches on the inst~nces.  P~tching h~s c~used downtime in the p~st. The comp~ny needs to m~ke the ~pplic~tion highly ~v~il~ble. Which solution will meet these requirements with the  LE;;ST development me?
  ;;.  Move the ~pplic~tion tier to ;;WS  L~mbd~ functions in the existing VPC. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer to distribute tr~ c ~cross the L~mbd~ functions. Use ;;m~zon Gu~rdDuty to sc~n the  L~mbd~ functions.  Migr~te the d~t~b~se to ;;m~zon  DocumentDB (with  MongoDB comp~tibility.
  B. Ch~nge the  EC2 inst~nce type to ~ sm~ller Gr~viton powered inst~nce type. Use the existing ;;MI to cre~te ~ l~unch templ~te for ~n ;;uto Sc~ling group. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer to distribute tr~ c ~cross the inst~nces in the ;;uto Sc~ling group. Set the ;;uto Sc~ling group to sc~le b~sed on CPU utiliz~tion.  Migr~te the d~t~b~se to ;;m~zon  Dyn~moDB.
  C.  Move the ~pplic~tion tier to cont~iners by using  Docker.  Run the cont~iners on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with  EC2 inst~nces. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer to distribute tr~ c ~cross the  ECS cluster. Con gure the  ECS cluster to sc~le b~sed on CPU utiliz~tion.  Migr~te the d~t~b~se to ;;m~zon  Neptune.
  D. Cre~te ~ now ;;MI th~t is con gured with ;;WS Systems  M~n~ger ;;gent (SSM ;;gent). Use the new ;;MI to cre~te ~ l~unch templ~te for ~n ;;uto Sc~ling group. Use sm~ller inst~nces in the ;;uto Sc~ling group. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer to distribute tr~ c ~cross the inst~nces in the ;;uto Sc~ling group. Set the ;;uto Sc~ling group to sc~le b~sed on CPU utiliz~tion.  Migr~te the d~t~b~se to ;;m~zon ;;uror~ MySQL.

 Correct ;;nswer: D
 D (100%)

 Question #300
 ;; comp~ny is pl~nning to migr~te sever~l ~pplic~tions to ;;WS. The comp~ny does not h~ve ~ good underst~nding of its entire ~pplic~tion est~te. The est~te consists of ~ mixture of physic~l m~chines ~nd VMs. One ~pplic~tion th~t the comp~ny will migr~te h~s m~ny dependencies th~t ~re sensitive to l~tency. The comp~ny is unsure wh~t ~ll the dependencies ~re.  However the comp~ny knows th~t the low-l~tency communic~tions use ~ custom  IP-b~sed protocol th~t runs on port  1000. The comp~ny w~nts to migr~te the ~pplic~tion ~nd these dependencies together to move ~ll the low-l~tency interf~ces to ;;WS ~t the s~me time. The comp~ny h~s inst~lled the ;;WS ;;pplic~tion  Discovery ;;gent ~nd h~s been collecting d~t~ for sever~l months. Wh~t should the comp~ny do to identify the dependencies th~t need to be migr~ted in the s~me ph~se ~s the ~pplic~tion?
  ;;. Use ;;WS  Migr~tion  Hub ~nd select the servers th~t host the ~pplic~tion. Visu~lize the network gr~ph to  nd servers th~t inter~ct with the ~pplic~tion. Turn on d~t~ explor~tion in ;;m~zon ;;then~. Query the d~t~ th~t is tr~nsferred between the servers to identify the servers th~t communic~te on port  1000.  Return to  Migr~tion  Hub. Cre~te ~ move group th~t is b~sed on the  ndings from the ;;then~ queries.
  B. Use ;;WS ;;pplic~tion  Migr~tion Service ~nd select the servers th~t host the ~pplic~tion. Visu~lize the network gr~ph to  nd servers th~t inter~ct with the ~pplic~tion. Con gure ;;pplic~tion  Migr~tion Service to l~unch test inst~nces for ~ll the servers th~t inter~ct with the ~pplic~tion.  Perform ~ccept~nce tests on the test inst~nces.  If no issues ~re identi ed, cre~te ~ move group th~t is b~sed on the tested servers.
  C. Use ;;WS  Migr~tion  Hub ~nd select the servers th~t host the ~pplic~tion. Turn on d~t~ explor~tion in  Network ;;ccess ;;n~lyzer. Use the Network ;;ccess ;;n~lyzer console to select the servers th~t host the ~pplic~tion. Select ~  Network ;;ccess Scope of port  1000 ~nd note the m~tching servers.  Return to  Migr~tion  Hub. Cre~te ~ move group th~t is b~sed on the  ndings from  Network ;;ccess ;;n~lyzer.
  D. Use ;;WS  Migr~tion  Hub ~nd select the servers th~t host the ~pplic~tion.  Push the ;;m~zon CloudW~lch ~gent to the identi ed servers by using the ;;WS ;;pplic~tion  Discovery ;;gent.  Export the CloudW~tch logs th~t the ~gents collect to ;;m~zon S3. Use ;;m~zon ;;then~ to query the logs to  nd servers th~t communic~te on port  1000.  Return to  Migr~tion  Hub Cre~te ~ move group th~t is b~sed on the  ndings from the ;;then~ queries.

 Correct ;;nswer: ;;
 ;; (92%)                                    8%

 Question #301
 ;; comp~ny is building ~n ~pplic~tion th~t will run on ~n ;;WS  L~mbd~ function.  Hundreds of customers will use the ~pplic~tion. The comp~ny w~nts to give e~ch customer ~ quot~ of requests for ~ speci c time period. The quot~s must m~tch customer us~ge p~tterns. Some customers must receive ~ higher quot~ for ~ shorter time period. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;m~zon ;;PI G~tew~y  REST ;;PI with ~ proxy integr~tion to invoke the  L~mbd~ function.  For e~ch customer, con gure ~n ;;PI G~tew~y us~ge pl~n th~t includes ~n ~ppropri~te request quot~. Cre~te ~n ;;PI key from the us~ge pl~n for e~ch user th~t the customer needs.
  B. Cre~te ~n ;;m~zon ;;PI G~tew~y  HTTP ;;PI with ~ proxy integr~tion to invoke the  L~mbd~ function.  For e~ch customer con gure ~n ;;PI G~tew~y us~ge pl~n th~t includes ~n ~ppropri~te request quot~ Con gure route-level throttling for e~ch us~ge pl~n. Cre~te ~n ;;PI  Key from the us~ge pl~n for e~ch user th~t the customer needs.
  C. Cre~te ~  L~mbd~ function ~li~s for e~ch customer.  Include ~ concurrency limit with ~n ~ppropri~te request quot~. Cre~te ~  L~mbd~ function URL for e~ch function ~li~s. Sh~re the  L~mbd~ function URL for e~ch ~li~s with the relev~nt customer.
  D. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) in ~ VPC. Con gure the  L~mbd~ function ~s ~ t~rget for the ;;LB. Con gure ~n ;;WS W;;F web ;;CL for the ;;LB.  For e~ch customer con gure ~ r~le-b~sed rule th~t includes ~n ~ppropri~te request quot~.

 Correct ;;nswer: ;;
 ;; (80%)                                  B (20%)

 Question #302
 ;; comp~ny is pl~nning to migr~te its on-premises VMw~re cluster of  120 VMs to ;;WS. The VMs h~ve m~ny different oper~ting systems ~nd m~ny custom softw~re p~ck~ges inst~lled. The comp~ny ~lso h~s ~n on-premises  NFS server th~t is  10 TB in size. The comp~ny h~s set up ~  10 Gbps ;;WS  Direct Connect connection to ;;WS for the migr~tion. Which solution will complete the migr~tion to ;;WS in the  LE;;ST ~mount of time?
  ;;.  Export the on-premises VMs ~nd copy them to ~n ;;m~zon S3 bucket. Use VM  Import/Export to cre~te ;;MIs from the VM im~ges th~t ~re stored in ;;m~zon S3. Order ~n ;;WS Snowb~ll  Edge device. Copy the  NFS server d~t~ to the device.  Restore the  NFS server d~t~ to ~n ;;m~zon EC2 inst~nce th~t h~s  NFS con gured.
  B. Con gure ;;WS ;;pplic~tion  Migr~tion Service with ~ connection to the VMw~re cluster. Cre~te ~ replic~tion job for the VMS. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system. Con gure ;;WS  D~t~Sync to copy the  NFS server d~t~ to the  EFS  le system over the Direct Connect connection.
  C.  Recre~te the VMs on ;;WS ~s ;;m~zon  EC2 inst~nces.  Inst~ll ~ll the required softw~re p~ck~ges. Cre~te ~n ;;m~zon  FSx for  Lustre  le system. Con gure ;;WS  D~t~Sync to copy the  NFS server d~t~ to the  FSx for  Lustre  le system over the  Direct Connect connection.
  D. Order two ;;WS Snowb~ll  Edge devices. Copy the VMs ~nd the  NFS server d~t~ to the devices.  Run VM  Import/Export ~fter the d~t~ from the devices is lo~ded to ~n ;;m~zon S3 bucket. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system. Copy the  NFS server d~t~ from ;;m~zon S3 to the  EFS  le system.

 Correct ;;nswer: B
 B (100%)

 Question #303
 ;;n online survey comp~ny runs its ~pplic~tion in the ;;WS Cloud. The ~pplic~tion is distributed ~nd consists of microservices th~t run in ~n ~utom~tic~lly sc~led ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster. The  ECS cluster is ~ t~rget for ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). The ;;LB is ~ custom origin for ~n ;;m~zon CloudFront distribution. The comp~ny h~s ~ survey th~t cont~ins sensitive d~t~. The sensitive d~t~ must be encrypted when it moves through the ~pplic~tion. The ~pplic~tion's d~t~-h~ndling microservice is the only microservice th~t should be ~ble to decrypt the d~t~ Which solution will meet these requirements?
  ;;. Cre~te ~ symmetric ;;WS  Key  M~n~gement Service (;;WS  KMS) key th~t is dedic~ted to the d~t~-h~ndling microservice. Cre~te ~  eld-level encryption pro le ~nd ~ con gur~tion. ;;ssoci~te the  KMS key ~nd the con gur~tion with the CloudFront c~che beh~vior.
  B. Cre~te ~n  RS;; key p~ir th~t is dedic~ted to the d~t~-h~nding microservice. Uplo~d the public key to the CloudFront distribution. Cre~te ~  eld-level encryption pro le ~nd ~ con gur~tion. ;;dd the con gur~tion to the CloudFront c~che beh~vior.
  C. Cre~te ~ symmetric ;;WS  Key  M~n~gement Service (;;WS  KMS) key th~t is dedic~ted to the d~t~-h~ndling microservice. Cre~te ~ L~mbd~@Edge function.  Progr~m the function to use the  KMS key to encrypt the sensitive d~t~.
  D. Cre~te ~n  RS;; key p~ir th~t is dedic~ted to the d~t~-h~ndling microservice. Cre~te ~  L~mbd~@Edge function.  Progr~m the function to use the priv~te key of the  RS;; key p~ir to encrypt the sensitive d~t~.

 Correct ;;nswer: B
 B (100%)

 Question #304
 ;; solutions ~rchitect is determining the  DNS str~tegy for ~n existing VPC. The VPC is provisioned to use the  10.24.34.0/24 CIDR block. The VPC ~lso uses ;;m~zon  Route 53  Resolver for  DNS.  New requirements m~nd~te th~t  DNS queries must use priv~te hosted zones. ;;ddition~lly inst~nces th~t h~ve public  IP ~ddresses must receive corresponding public hostn~mes Which solution will meet these requirements to ensure th~t the dom~in n~mes ~re correctly resolved within the VPC?
  ;;. Cre~te ~ priv~te hosted zone. ;;ctiv~te the en~bleDnsSupport ~ttribute ~nd the en~bleDnsHostn~mes ~ttribute for the VPC. Upd~te the VPC DHCP options set to include dom~in-n~me-servers=10.24.34.2.
  B. Cre~te ~ priv~te hosted zone ;;ssoci~te the priv~te hosted zone with the VPC. ;;ctiv~te the en~bleDnsSupport ~ttribute ~nd the en~bleDnsHostn~mes ~ttribute for the VPC. Cre~te ~ new VPC  DHCP options set, ~nd con gure dom~in-n~me-servers=;;m~zonProvidedDNS. ;;ssoci~te the new  DHCP options set with the VPC.
  C.  De~ctiv~te the en~bleDnsSupport ~ttribute for the VP;;ctiv~te the en~bleDnsHostn~mes ~ttribute for the VPCre~te ~ new VPC  DHCP options set, ~nd con gure dom~n-n~me-servers=10.24.34.2. ;;ssoci~te the new  DHCP options set with the VPC.
  D. Cre~te ~ priv~te hosted zone. ;;ssoci~te the priv~te hosted zone with the VPC. ;;ctiv~te the en~bleDnsSupport ~ttribute for the VPC. De~ctiv~te the en~bleDnsHostn~mes ~ttribute for the VPC. Upd~te the VPC  DHCP options set to include dom~in-n~me- servers=;;m~zonProvidedDNS.

 Correct ;;nswer: B
 B (100%)

 Question #305
 ;; d~t~ ~n~lytics comp~ny h~s ~n ;;m~zon  Redshift cluster th~t consists of sever~l reserved nodes. The cluster is experiencing unexpected bursts of us~ge bec~use ~ te~m of employees is compiling ~ deep ~udit ~n~lysis report. The queries to gener~te the report ~re complex re~d queries ~nd ~re CPU intensive. Business requirements dict~te th~t the cluster must be ~ble to service re~d ~nd write queries ~t ~ll times. ;; solutions ~rchitect must devise ~ solution th~t ~ccommod~tes the bursts of us~ge. Which solution meets these requirements  MOST cost-effectively?
  ;;.  Provision ~n ;;m~zon  EMR cluster O o~d the complex d~t~ processing t~sks.
  B.  Deploy ~n ;;WS  L~mbd~ function to ~dd c~p~city to the ;;m~zon  Redshift cluster by using ~ cl~ssic resize oper~tion when the cluster’s CPU metrics in ;;m~zon CloudW~tch re~ch 80%.
  C.  Deploy ~n ;;WS  L~mbd~ function to ~dd c~p~city to the ;;m~zon  Redshift cluster by using ~n el~stic resize oper~tion when the cluster’s CPU metrics in ;;m~zon CloudW~tch re~ch 80%.
  D. Turn on the Concurrency Sc~ling fe~ture for the ;;m~zon  Redshift cluster.

 Correct ;;nswer: D
 D (100%)

 Question #306
 ;; rese~rch center is migr~ting to the ;;WS Cloud ~nd h~s moved its on-premises  1  PB object stor~ge to ~n ;;m~zon S3 bucket. One hundred scientists ~re using this object stor~ge to store their work-rel~ted documents.  E~ch scientist h~s ~ person~l folder on the object store. ;;ll the scientists ~re members of ~ single  I;;M user group. The rese~rch center's compli~nce o cer is worried th~t scientists will be ~ble to ~ccess e~ch other's work. The rese~rch center h~s ~ strict oblig~tion to report on which scientist ~ccesses which documents. The te~m th~t is responsible for these reports h~s little ;;WS experience ~nd w~nts ~ re~dy-to-use solution th~t minimizes oper~tion~l overhe~d. Which combin~tion of ~ctions should ~ solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;. Cre~te ~n identity policy th~t gr~nts the user re~d ~nd write ~ccess. ;;dd ~ condition th~t speci es th~t the S3 p~ths must be pre xed with $(~ws:usern~me). ;;pply the policy on the scientists’  I;;M user group.
  B. Con gure ~ tr~il with ;;WS CloudTr~il to c~pture ~ll object-level events in the S3 bucket. Store the tr~il output in ~nother S3 bucket. Use ;;m~zon ;;then~ to query the logs ~nd gener~te reports.
  C.  En~ble S3 server ~ccess logging. Con gure ~nother S3 bucket ~s the t~rget for log delivery. Use ;;m~zon ;;then~ to query the logs ~nd gener~te reports.
  D. Cre~te ~n S3 bucket policy th~t gr~nts re~d ~nd write ~ccess to users in the scientists’  I;;M user group.
  E. Con gure ~ tr~il with ;;WS CloudTr~il to c~pture ~ll object-level events in the S3 bucket ~nd write the events to ;;m~zon CloudW~tch. Use the ;;m~zon ;;then~ CloudW~tch connector to query the logs ~nd gener~te reports.

 Correct ;;nswer: ;;B
 ;;B (64%)                         BD (18%)       ;;C (18%)

 Question #307
 ;; comp~ny uses ;;WS Org~niz~tions to m~n~ge ~ multi-~ccount structure. The comp~ny h~s hundreds of ;;WS ~ccounts ~nd expects the number of ~ccounts to incre~se. The comp~ny is building ~ new ~pplic~tion th~t uses  Docker im~ges. The comp~ny will push the  Docker im~ges to ;;m~zon  El~stic Cont~iner  Registry (;;m~zon  ECR). Only ~ccounts th~t ~re within the comp~ny’s org~niz~tion should h~ve ~ccess to the im~ges. The comp~ny h~s ~ CI/CD process th~t runs frequently. The comp~ny w~nts to ret~in ~ll the t~gged im~ges.  However, the comp~ny w~nts to ret~in only the  ve most recent unt~gged im~ges. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ priv~te repository in ;;m~zon  ECR. Cre~te ~ permissions policy for the repository th~t ~llows only required  ECR oper~tions.  Include ~ condition to ~llow the  ECR oper~tions if the v~lue of the ~ws:Princip~lOrglD condition key is equ~l to the  ID of the comp~ny’s org~niz~tion. ;;dd ~ lifecycle rule to the  ECR repository th~t deletes ~ll unt~gged im~ges over the count of  ve
  B. Cre~te ~ public repository in ;;m~zon  ECR. Cre~te ~n  I;;M role in the  ECR ~ccount. Set permissions so th~t ~ny ~ccount c~n ~ssume the role if the v~lue of the ~ws:Princip~lOrglD condition key is equ~l to the  ID of the comp~ny’s org~niz~tion. ;;dd ~ lifecycle rule to the  ECR repository th~t deletes ~ll unt~gged im~ges over the count of  ve.
  C. Cre~te ~ priv~te repository in ;;m~zon  ECR. Cre~te ~ permissions policy for the repository th~t includes only required  ECR oper~tions. Include ~ condition to ~llow the  ECR oper~tions for ~ll ~ccount  IDs in the org~niz~tion Schedule ~ d~ily ;;m~zon  EventBridge rule to invoke ~n ;;WS  L~mbd~ function th~t deletes ~ll unt~gged im~ges over the count of  ve.
  D. Cre~te ~ public repository in ;;m~zon  ECR. Con gure ;;m~zon  ECR to use ~n interf~ce VPC endpoint with ~n endpoint policy th~t includes the required permissions for im~ges th~t the comp~ny needs to pull.  Include ~ condition to ~llow the  ECR oper~tions for ~ll ~ccount  IDs in the comp~ny’s org~niz~tion. Schedule ~ d~ily ;;m~zon  EventBridge rule to invoke ~n ;;WS  L~mbd~ function th~t deletes ~ll unt~gged im~ges over the count of  ve.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #308
 ;; solutions ~rchitect is reviewing ~ comp~ny's process for t~king sn~pshots of ;;m~zon  RDS  DB inst~nces. The comp~ny t~kes ~utom~tic sn~pshots every d~y ~nd ret~ins the sn~pshots for 7 d~ys. The solutions ~rchitect needs to recommend ~ solution th~t t~kes sn~pshots every 6 hours ~nd ret~ins the sn~pshots for 30 d~ys. The comp~ny uses ;;WS Org~niz~tions to m~n~ge ~ll of its ;;WS ~ccounts. The comp~ny needs ~ consolid~ted view of the he~lth of the  RDS sn~pshots. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Turn on the cross-~ccount m~n~gement fe~ture in ;;WS  B~ckup. Cre~te ~ b~ckup pl~n th~t speci es the frequency ~nd retention requirements. ;;dd ~ t~g to the  DB inst~nces. ;;pply the b~ckup pl~n by using t~gs. Use ;;WS  B~ckup to monitor the st~tus of the b~ckups.
  B. Turn on the cross-~ccount m~n~gement fe~ture in ;;m~zon  RDS. Cre~te ~ sn~pshot glob~l policy th~t speci es the frequency ~nd retention requirements. Use the  RDS console in the m~n~gement ~ccount to monitor the st~tus of the b~ckups.
  C. Turn on the cross-~ccount m~n~gement fe~ture in ;;WS CloudForm~tion.  From the m~n~gement ~ccount, deploy ~ CloudForm~tion st~ck set th~t cont~ins ~ b~ckup pl~n from ;;WS  B~ckup th~t speci es the frequency ~nd retention requirements. Cre~te ~n ;;WS  L~mbd~ function in the m~n~gement ~ccount to monitor the st~tus of the b~ckups. Cre~te ~n ;;m~zon  EventBridge rule in e~ch ~ccount to run the  L~mbd~ function on ~ schedule.
  D. Con gure ;;WS  B~ckup in e~ch ~ccount. Cre~te ~n ;;m~zon  D~t~  Lifecycle  M~n~ger lifecycle policy th~t speci es the frequency ~nd retention requirements. Specify the  DB inst~nces ~s the t~rget resource Use the ;;m~zon  D~t~  Lifecycle  M~n~ger console in e~ch member ~ccount to monitor the st~tus of the b~ckups.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #309
 ;; comp~ny is using ;;WS Org~niz~tions with ~ multi-~ccount ~rchitecture. The comp~ny's current security con gur~tion for the ~ccount ~rchitecture includes SCPs, resource-b~sed policies, identity-b~sed policies, trust policies, ~nd session policies. ;; solutions ~rchitect needs to ~llow ~n  I;;M user in ;;ccount ;; to ~ssume ~ role in ;;ccount  B. Which combin~tion of steps must the solutions ~rchitect t~ke to meet this requirement? (Choose three.)
  ;;. Con gure the SCP for ;;ccount ;; to ~llow the ~ction.
  B. Con gure the resource-b~sed policies to ~llow the ~ction.
  C. Con gure the identity-b~sed policy on the user in ;;ccount ;; to ~llow the ~ction.
  D. Con gure the identity-b~sed policy on the user in ;;ccount  B to ~llow the ~ction.
  E. Con gure the trust policy on the t~rget role in ;;ccount  B to ~llow the ~ction.
  F. Con gure the session policy to ~llow the ~ction ~nd to be p~ssed progr~mm~tic~lly by the GetSessionToken ;;PI oper~tion.

 Correct ;;nswer: ;;CE
 CEF (50%)                        BCE (31%)           ;;CE (19%)

 Question #310
 ;; comp~ny w~nts to use ;;m~zon S3 to b~ck up its on-premises  le stor~ge solution. The comp~ny’s on-premises  le stor~ge solution supports NFS, ~nd the comp~ny w~nts its new solution to support  NFS. The comp~ny w~nts to ~rchive the b~ckup  les ~fter 5 d~ys.  If the comp~ny needs ~rchived  les for dis~ster recovery, the comp~ny is willing to w~it ~ few d~ys for the retriev~l of those  les. Which solution meets these requirements  MOST cost-effectively?
  ;;.  Deploy ~n ;;WS Stor~ge G~tew~y  le g~tew~y th~t is ~ssoci~ted with ~n S3 bucket.  Move the  les from the on-premises  le stor~ge solution to the  le g~tew~y. Cre~te ~n S3  Lifecycle rule to move the  les to S3 St~nd~rd-Infrequent ;;ccess (S3 St~nd~rd-I;;) ~fter 5 d~ys.
  B.  Deploy ~n ;;WS Stor~ge G~tew~y volume g~tew~y th~t is ~ssoci~ted with ~n S3 bucket.  Move the  les from the on-premises  le stor~ge solution to the volume g~tew~y. Cre~te ~n S3  Lifecycle rule to move the  les to S3 Gl~cier  Deep ;;rchive ~fter 5 d~ys.
  C.  Deploy ~n ;;WS Stor~ge G~tew~y t~pe g~tew~y th~t is ~ssoci~ted with ~n S3 bucket.  Move the  les from the on-premises  le stor~ge solution to the t~pe g~tew~y. Cre~te ~n S3  Lifecycle rule to move the  les to S3 St~nd~rd-Infrequent ;;ccess (S3 St~nd~rd-I;;) ~fter 5 d~ys.
  D.  Deploy ~n ;;WS Stor~ge G~tew~y  le g~tew~y th~t is ~ssoci~ted with ~n S3 bucket.  Move the  les from the on-premises  le stor~ge solution to the  le g~tew~y. Cre~te ~n S3  Lifecycle rule to move the  les to S3 Gl~cier  Deep ;;rchive ~fter 5 d~ys.

 Correct ;;nswer: D
 D (100%)

 Question #311
 ;; comp~ny runs its ~pplic~tion on ;;m~zon  EC2 inst~nces ~nd ;;WS  L~mbd~ functions. The  EC2 inst~nces experience ~ continuous ~nd st~ble lo~d. The  L~mbd~ functions experience ~ v~ried ~nd unpredict~ble lo~d. The ~pplic~tion includes ~ c~ching l~yer th~t uses ~n ;;m~zon  MemoryDB for  Redis cluster. ;; solutions ~rchitect must recommend ~ solution to minimize the comp~ny's over~ll monthly costs. Which solution will meet these requirements?
  ;;.  Purch~se ~n  EC2 inst~nce S~vings  Pl~n to cover the  EC2 inst~nces.  Purch~se ~ Compute S~vings  Pl~n for  L~mbd~ to cover the minimum expected consumption of the  L~mbd~ functions.  Purch~se reserved nodes to cover the  MemoryDB c~che nodes.
  B.  Purch~se ~ Compute S~vings  Pl~n to cover the  EC2 inst~nces.  Purch~se  L~mbd~ reserved concurrency to cover the expected  L~mbd~ us~ge.  Purch~se reserved nodes to cover the  MemoryDB c~che nodes.
  C.  Purch~se ~ Compute S~vings  Pl~n to cover the entire expected cost of the  EC2 inst~nces,  L~mbd~ functions, ~nd  MemoryDB c~che nodes.
  D.  Purch~se ~ Compute S~vings  Pl~n to cover the  EC2 inst~nces ~nd the  MemoryDB c~che nodes.  Purch~se  L~mbd~ reserved concurrency to cover the expected  L~mbd~ us~ge.

 Correct ;;nswer: C
 ;; (82%)                                  B (18%)

 Question #312
 ;; comp~ny is l~unching ~ new online g~me on ;;m~zon  EC2 inst~nces. The g~me must be ~v~il~ble glob~lly. The comp~ny pl~ns to run the g~me in three ;;WS  Regions us-e~st-1, eu-west-1, ~nd ~p-southe~st-1. The g~me's le~derbo~rds, pl~yer inventory ~nd event st~tus must be ~v~il~ble ~cross  Regions. ;; solutions ~rchitect must design ~ solution th~t will give ~ny  Region the ~bility to sc~le to h~ndle the lo~d of ~ll  Regions. ;;ddition~lly, users must ~utom~tic~lly connect to the  Region th~t provides the le~st l~tency. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n  EC2 Spot  Fleet. ;;tt~ch the Spot  Fleet to ~  Network  Lo~d  B~l~ncer (NLB) in e~ch  Region. Cre~te ~n ;;WS Glob~l ;;cceler~tor  IP ~ddress th~t points to the  NLB. Cre~te ~n ;;m~zon  Route 53 l~tency-b~sed routing entry for the Glob~l ;;cceler~tor  IP ~ddress. S~ve the g~me met~d~t~ to ~n ;;m~zon  RDS for  MySQL  DB inst~nce in e~ch  Region. Set up ~ re~d replic~ in the other  Regions.
  B. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces ;;tt~ch the ;;uto Sc~ling group to ~  Network  Lo~d  B~l~ncer (NLB) in e~ch  Region.  For e~ch  Region, cre~te ~n ;;m~zon  Route 53 entry th~t uses geoproximity routing ~nd points to the  NLB in th~t  Region. S~ve the g~me met~d~t~ to  MySQL d~t~b~ses on  EC2 inst~nces in e~ch  Region. Set up replic~tion between the d~t~b~se  EC2 inst~nces in e~ch  Region.
  C. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces. ;;tt~ch the ;;uto Sc~ling group to ~  Network  Lo~d  B~l~ncer (NLB) in e~ch  Region.  For e~ch  Region, cre~te ~n ;;m~zon  Route 53 entry th~t uses l~tency-b~sed routing ~nd points to the  NLB in th~t  Region. S~ve the g~me met~d~t~ to ~n ;;m~zon  Dyn~moDB glob~l t~ble.
  D. Use  EC2 Glob~l View.  Deploy the  EC2 inst~nces to e~ch  Region. ;;tt~ch the inst~nces to ~  Network  Lo~d  B~l~ncer (NLB).  Deploy ~  DNS server on ~n  EC2 inst~nce in e~ch  Region. Set up custom logic on e~ch  DNS server to redirect the user to the  Region th~t provides the lowest l~tency. S~ve the g~me met~d~t~ to ~n ;;m~zon ;;uror~ glob~l d~t~b~se.

 Correct ;;nswer: C
 C (100%)

 Question #313
 ;; comp~ny is deploying ~ third-p~rty  rew~ll ~ppli~nce solution from ;;WS  M~rketpl~ce to monitor ~nd protect tr~ c th~t le~ves the comp~ny's ;;WS environments. The comp~ny w~nts to deploy this ~ppli~nce into ~ sh~red services VPC ~nd route ~ll outbound internet-bound tr~ c through the ~ppli~nces. ;; solutions ~rchitect needs to recommend ~ deployment method th~t prioritizes reli~bility ~nd minimizes f~ilover time between  rew~ll ~ppli~nces within ~ single ;;WS  Region. The comp~ny h~s set up routing from the sh~red services VPC to other VPCs. Which steps should the solutions ~rchitect recommend to meet these requirements? (Choose three.)
  ;;.  Deploy two  rew~ll ~ppli~nces into the sh~red services VPC, e~ch in ~ sep~r~te ;;v~il~bility Zone.
  B. Cre~te ~ new  Network  Lo~d  B~l~ncer in the sh~red services VPC. Cre~te ~ new t~rget group, ~nd ~tt~ch it to the new  Network  Lo~d B~l~ncer. ;;dd e~ch of the  rew~ll ~ppli~nce inst~nces to the t~rget group.
  C. Cre~te ~ new G~tew~y  Lo~d  B~l~ncer in the sh~red services VPCre~te ~ new t~rget group, ~nd ~tt~ch it to the new G~tew~y  Lo~d  B~l~ncer ;;dd e~ch of the  rew~ll ~ppli~nce inst~nces to the t~rget group.
  D. Cre~te ~ VPC interf~ce endpoint. ;;dd ~ route to the route t~ble in the sh~red services VPC.  Design~te the new endpoint ~s the next hop for tr~ c th~t enters the sh~red services VPC from other VPCs.
  E.  Deploy two  rew~ll ~ppli~nces into the sh~red services VPC, e~ch in the s~me ;;v~il~bility Zone.
  F. Cre~te ~ VPC G~tew~y  Lo~d  B~l~ncer endpoint. ;;dd ~ route to the route t~ble in the sh~red services VPC.  Design~te the new endpoint ~s the next hop for tr~ c th~t enters the sh~red services VPC from other VPCs.

 Correct ;;nswer: ;;CF
 ;;CF (80%)                               13%      7%

 Question #314
 ;; solutions ~rchitect needs to migr~te ~n on-premises leg~cy ~pplic~tion to ;;WS. The ~pplic~tion runs on two servers behind ~ lo~d b~l~ncer. The ~pplic~tion requires ~ license  le th~t is ~ssoci~ted with the  M;;C ~ddress of the server's network ~d~pter  It t~kes the softw~re vendor  12 hours to send new license  les. The ~pplic~tion ~lso uses con gur~tion  les with ~ st~tic  IP ~ddress to ~ccess ~ d~t~b~se server, host n~mes ~re not supported. Given these requirements, which combin~tion of steps should be t~ken to implement highly ~v~il~ble ~rchitecture for the ~pplic~tion servers in ;;WS? (Choose two.)
  ;;. Cre~te ~ pool of  ENIs.  Request license  les from the vendor for the pool, ~nd store the license  les in ;;m~zon S3. Cre~te ~ bootstr~p ~utom~tion script to downlo~d ~ license  le ~nd ~tt~ch the corresponding  ENI to ~n ;;m~zon  EC2 inst~nce.
  B. Cre~te ~ pool of  ENIs.  Request license  les from the vendor for the pool, store the license  les on ~n ;;m~zon  EC2 inst~nce. Cre~te ~n ;;MI from the inst~nce ~nd use this ;;MI for ~ll future  EC2 inst~nces.
  C. Cre~te ~ bootstr~p ~utom~tion script to request ~ new license  le from the vendor .When the response is received, ~pply the license  le to ~n ;;m~zon  EC2 inst~nce.
  D.  Edit the bootstr~p ~utom~tion script to re~d the d~t~b~se server  IP ~ddress from the ;;WS Systems  M~n~ger  P~r~meter Store, ~nd inject the v~lue into the loc~l con gur~tion  les.
  E.  Edit ~n ;;m~zon  EC2 inst~nce to include the d~t~b~se server  IP ~ddress in the con gur~tion  les ~nd re-cre~te the ;;MI to use for ~ll future EC2 st~nces.

 Correct ;;nswer: ;;D
 ;;D (100%)

 Question #315
 ;; comp~ny runs its s~les reporting ~pplic~tion in ~n ;;WS  Region in the United St~tes. The ~pplic~tion uses ~n ;;m~zon ;;PI G~tew~y  Region~l ;;PI ~nd ;;WS  L~mbd~ functions to gener~te on-dem~nd reports from d~t~ in ~n ;;m~zon  RDS for  MySQL d~t~b~se. The frontend of the ~pplic~tion is hosted on ;;m~zon S3 ~nd is ~ccessed by users through ~n ;;m~zon CloudFront distribution. The comp~ny is using ;;m~zon  Route 53 ~s the  DNS service for the dom~in.  Route 53 is con gured with ~ simple routing policy to route tr~ c to the ;;PI G~tew~y ;;PI. In the next 6 months, the comp~ny pl~ns to exp~nd oper~tions to  Europe.  More th~n 90% of the d~t~b~se tr~ c is re~d-only tr~ c. The comp~ny h~s ~lre~dy deployed ~n ;;PI G~tew~y ;;PI ~nd  L~mbd~ functions in the new  Region. ;; solutions ~rchitect must design ~ solution th~t minimizes l~tency for users who downlo~d reports. Which solution will meet these requirements?
  ;;. Use ~n ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) t~sk with full lo~d to replic~te the prim~ry d~t~b~se in the origin~l  Region to the d~t~b~se in the new  Region. Ch~nge the  Route 53 record to l~tency-b~sed routing to connect to the ;;PI G~tew~y ;;PI.
  B. Use ~n ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) t~sk with full lo~d plus ch~nge d~t~ c~pture (CDC) to replic~te the prim~ry d~t~b~se in the origin~l  Region to the d~t~b~se in the new  Region. Ch~nge the  Route 53 record to geoloc~tion routing to connect to the ;;PI G~tew~y ;;PI.
  C. Con gure ~ cross-Region re~d replic~ for the  RDS d~t~b~se in the new  Region Ch~nge the  Route 53 record to l~tency-b~sed routing to connect to the ;;PI G~tew~y ;;PI.
  D. Con gure ~ cross-Region re~d replic~ for the  RDS d~t~b~se in the new  Region. Ch~nge the  Route 53 record to geoloc~tion routing to connect to the ;;PI G~tew~y ;;PI.

 Correct ;;nswer: D
 C (93%)                                     7%

 Question #316
 ;; softw~re comp~ny needs to cre~te short-lived test environments to test pull requests ~s p~rt of its development process.  E~ch test environment consists of ~ single ;;m~zon  EC2 inst~nce th~t is in ~n ;;uto Sc~ling group. The test environments must be ~ble to communic~te with ~ centr~l server to report test results. The centr~l server is loc~ted in ~n on-premises d~t~ center. ;; solutions ~rchitect must implement ~ solution so th~t the comp~ny c~n cre~te ~nd delete test environments without ~ny m~nu~l intervention. The comp~ny h~s cre~ted ~ tr~nsit g~tew~y with ~ VPN ~tt~chment to the on-premises network. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~n ;;WS CloudForm~tion templ~te th~t cont~ins ~ tr~nsit g~tew~y ~tt~chment ~nd rel~ted routing con gur~tions. Cre~te ~ CloudForm~tion st~ck set th~t includes this templ~te. Use CloudForm~tion St~ckSets to deploy ~ new st~ck for e~ch VPC in the ~ccount. Deploy ~ new VPC for e~ch test environment.
  B. Cre~te ~ single VPC for the test environments.  Include ~ tr~nsit g~tew~y ~tt~chment ~nd rel~ted routing con gur~tions. Use ;;WS CloudForm~tion to deploy ~ll test environments into the VPC.
  C. Cre~te ~ new OU in ;;WS Org~niz~tions for testing. Cre~te ~n ;;WS CioudForm~tion templ~te th~t cont~ins ~ VPC, necess~ry networking resources, ~ tr~nsit g~tew~y ~tt~chment, ~nd rel~ted routing con gur~tions. Cre~te ~ CloudForm~tion st~ck set th~t includes this templ~te. Use CloudForm~tion St~ckSets for deployments into e~ch ~ccount under the testing OU. Cre~te ~ new ~ccount for e~ch test environment.
  D. Convert the test environment  EC2 inst~nces into  Docker im~ges. Use ;;WS CloudForm~tion to con gure ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster in ~ new VPC, cre~te ~ tr~nsit g~tew~y ~tt~chment, ~nd cre~te rel~ted routing con gur~tions. Use  Kubernetes to m~n~ge the deployment ~nd lifecycle of the test environments.

 Correct ;;nswer: B
 B (100%)

 Question #317
 ;; comp~ny is deploying ~ new ;;PI to ;;WS. The ;;PI uses ;;m~zon ;;PI G~tew~y with ~  Region~l ;;PI endpoint ~nd ~n ;;WS  L~mbd~ function for hosting. The ;;PI retrieves d~t~ from ~n extern~l vendor ;;PI, stores d~t~ in ~n ;;m~zon  Dyn~moDB glob~l t~ble, ~nd retrieves d~t~ from the Dyn~moDB glob~l t~ble The ;;PI key for the vendor's ;;PI is stored in ;;WS Secrets  M~n~ger ~nd is encrypted with ~ customer m~n~ged key in ;;WS Key  M~n~gement Service (;;WS  KMS). The comp~ny h~s deployed its own ;;PI into ~ single ;;WS  Region. ;; solutions ~rchitect needs to ch~nge the ;;PI components of the comp~ny’s ;;PI to ensure th~t the components c~n run ~cross multiple  Regions in ~n ~ctive-~ctive con gur~tion. Which combin~tion of ch~nges will meet this requirement with the  LE;;ST oper~tion~l overhe~d? (Choose three.)
  ;;.  Deploy the ;;PI to multiple  Regions. Con gure ;;m~zon  Route 53 with custom dom~in n~mes th~t route tr~ c to e~ch  Region~l ;;PI endpoint.  Implement ~  Route 53 multiv~lue ~nswer routing policy.
  B. Cre~te ~ new  KMS multi-Region customer m~n~ged key. Cre~te ~ new  KMS customer m~n~ged replic~ key in e~ch in-scope  Region.
  C.  Replic~te the existing Secrets  M~n~ger secret to other  Regions.  For e~ch in-scope  Region's replic~ted secret, select the ~ppropri~te  KMS key.
  D. Cre~te ~ new ;;WS m~n~ged  KMS key in e~ch in-scope  Region. Convert ~n existing key to ~ multiRegion key. Use the multi-Region key in other  Regions.
  E. Cre~te ~ new Secrets  M~n~ger secret in e~ch in-scope  Region. Copy the secret v~lue from the existing  Region to the new secret in e~ch in- scope  Region.
  F.  Modify the deployment process for the  L~mbd~ function to repe~t the deployment ~cross in-scope  Regions. Turn on the multi-Region option for the existing ;;PI. Select the  L~mbd~ function th~t is deployed in e~ch  Region ~s the b~ckend for the multi-Region ;;PI.

 Correct ;;nswer: ;;BC
 ;;BC (70%)                                BCF (30%)

 Question #318
 ;;n online ret~il comp~ny hosts its st~teful web-b~sed ~pplic~tion ~nd  MySQL d~t~b~se in ~n on-premises d~t~ center on ~ single server. The comp~ny w~nts to incre~se its customer b~se by conducting more m~rketing c~mp~igns ~nd promotions.  In prep~r~tion, the comp~ny w~nts to migr~te its ~pplic~tion ~nd d~t~b~se to ;;WS to incre~se the reli~bility of its ~rchitecture. Which solution should provide the  HIGHEST level of reli~bility?
  ;;.  Migr~te the d~t~b~se to ~n ;;m~zon  RDS  MySQL  Multi-;;Z  DB inst~nce.  Deploy the ~pplic~tion in ~n ;;uto Sc~ling group on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Store sessions in ;;m~zon  Neptune
  B.  Migr~te the d~t~b~se to ;;m~zon ;;uror~  MySQL.  Deploy the ~pplic~tion in ~n ;;uto Sc~ling group on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Store sessions in ~n ;;m~zon  El~stiC~che for  Redis replic~tion group.
  C.  Migr~te the d~t~b~se to ;;m~zon  DocumentDB (with  MongoDB comp~tibility).  Deploy the ~pplic~tion in ~n ;;uto Sc~ling group on ;;m~zon EC2 inst~nces behind ~  Network  Lo~d  B~l~ncer Store sessions in ;;m~zon  Kinesis  D~t~  Firehose.
  D.  Migr~te the d~t~b~se to ~n ;;m~zon  RDS  M~ri~DB  Multi-;;Z  DB inst~nce.  Deploy the ~pplic~tion in ~n ;;uto Sc~ling group on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Store sessions in ;;m~zon  El~stiC~che for  Memc~ched.

 Correct ;;nswer: B
 B (100%)

 Question #319
 ;; comp~ny’s solutions ~rchitect needs to provide secure  Remote  Desktop connectivity to users for ;;m~zon  EC2 Windows inst~nces th~t ~re hosted in ~ VPC. The solution must integr~te centr~lized user m~n~gement with the comp~ny's on-premises ;;ctive  Directory. Connectivity to the VPC is through the internet. The comp~ny h~s h~rdw~re th~t c~n be used to est~blish ~n ;;WS Site-to-Site VPN connection. Which solution will meet these requirements  MOST cost-effectively?
  ;;.  Deploy ~ m~n~ged ;;ctive  Directory by using ;;WS  Directory Service for  Microsoft ;;ctive  Directory.  Est~blish ~ trust with the on-premises ;;ctive  Directory.  Deploy ~n  EC2 inst~nce ~s ~ b~stion host in the VPC.  Ensure th~t the  EC2 inst~nce is joined to the dom~in. Use the b~stion host to ~ccess the t~rget inst~nces through  RDP.
  B. Con gure ;;WS  I;;M  Identity Center (;;WS Single Sign-On) to integr~te with the on-premises ;;ctive  Directory by using the ;;WS  Directory Service for  Microsoft ;;ctive  Directory ;;D Connector. Con gure permission sets ~g~inst user groups for ~ccess to ;;WS Systems  M~n~ger. Use Systems  M~n~ger  Fleet  M~n~ger to ~ccess the t~rget inst~nces through  RDP.
  C.  Implement ~ VPN between the on-premises environment ~nd the t~rget VPEnsure th~t the t~rget inst~nces ~re joined to the on-premises ;;ctive  Directory dom~in over the VPN connection. Con gure  RDP ~ccess through the VPN. Connect from the comp~ny’s network to the t~rget inst~nces.
  D.  Deploy ~ m~n~ged ;;ctive  Directory by using ;;WS  Directory Service for  Microsoft ;;ctive  Directory.  Est~blish ~ trust with the on-premises ;;ctive  Directory.  Deploy ~  Remote  Desktop G~tew~y on ;;WS by using ~n ;;WS Quick St~rt.  Ensure th~t the  Remote  Desktop G~tew~y is joined to the dom~in. Use the  Remote  Desktop G~tew~y to ~ccess the t~rget inst~nces through  RDP.

 Correct ;;nswer: C
 B (68%)                              C (23%)        9%

 Question #320
 ;; comp~ny's compli~nce ~udit reve~ls th~t some ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes th~t were cre~ted in ~n ;;WS ~ccount were not encrypted. ;; solutions ~rchitect must implement ~ solution to encrypt ~ll new  EBS volumes ~t rest. Which solution will meet this requirement with the  LE;;ST effort?
  ;;. Cre~te ~n ;;m~zon  EventBridge rule to detect the cre~tion of unencrypted  EBS volumes.  Invoke ~n ;;WS  L~mbd~ function to delete noncompli~nt volumes.
  B. Use ;;WS ;;udit  M~n~ger with d~t~ encryption.
  C. Cre~te ~n ;;WS Con g rule to detect the cre~tion of ~ new  EBS volume.  Encrypt the volume by using ;;WS Systems  M~n~ger ;;utom~tion.
  D. Turn on  EBS encryption by def~ult in ~ll ;;WS  Regions.

 Correct ;;nswer: D
 D (86%)                                    14%

 Question #321
 ;; rese~rch comp~ny is running d~ily simul~tions in the ;;WS Cloud to meet high dem~nd. The simul~tions run on sever~l hundred ;;m~zon  EC2 inst~nces th~t ~re b~sed on ;;m~zon  Linux 2. Occ~sion~lly, ~ simul~tion gets stuck ~nd requires ~ cloud oper~tions engineer to solve the problem by connecting to ~n  EC2 inst~nce through SSH. Comp~ny policy st~tes th~t no  EC2 inst~nce c~n use the s~me SSH key ~nd th~t ~ll connections must be logged in ;;WS CloudTr~il. How c~n ~ solutions ~rchitect meet these requirements?
  ;;.  L~unch new  EC2 inst~nces, ~nd gener~te ~n individu~l SSH key for e~ch inst~nce. Store the SSH key in ;;WS Secrets  M~n~ger. Cre~te ~ new I;;M policy, ~nd ~tt~ch it to the engineers’  I;;M role with ~n ;;llow st~tement for the GetSecretV~lue ~ction.  Instruct the engineers to fetch the SSH key from Secrets  M~n~ger when they connect through ~ny SSH client.
  B. Cre~te ~n ;;WS Systems  M~n~ger document to run comm~nds on  EC2 inst~nces to set ~ new unique SSH key. Cre~te ~ new  I;;M policy, ~nd ~tt~ch it to the engineers’  I;;M role with ~n ;;llow st~tement to run Systems  M~n~ger documents.  Instruct the engineers to run the document to set ~n SSH key ~nd to connect through ~ny SSH client.
  C.  L~unch new  EC2 inst~nces without setting up ~ny SSH key for the inst~nces. Set up  EC2  Inst~nce Connect on e~ch inst~nce. Cre~te ~ new I;;M policy, ~nd ~tt~ch it to the engineers’  I;;M role with ~n ;;llow st~tement for the SendSSHPublicKey ~ction.  Instruct the engineers to connect to the inst~nce by using ~ browser-b~sed SSH client from the  EC2 console.
  D. Set up ;;WS Secrets  M~n~ger to store the  EC2 SSH key. Cre~te ~ new ;;WS  L~mbd~ function to cre~te ~ new SSH key ~nd to c~ll ;;WS Systems  M~n~ger Session  M~n~ger to set the SSH key on the  EC2 inst~nce. Con gure Secrets  M~n~ger to use the  L~mbd~ function for ~utom~tic rot~tion once d~ily.  Instruct the engineers to fetch the SSH key from Secrets  M~n~ger when they connect through ~ny SSH client.

 Correct ;;nswer: C
 C (100%)

 Question #322
 ;; comp~ny is migr~ting mobile b~nking ~pplic~tions to run on ;;m~zon  EC2 inst~nces in ~ VPC.  B~ckend service ~pplic~tions run in ~n on- premises d~t~ center. The d~t~ center h~s ~n ;;WS  Direct Connect connection into ;;WS. The ~pplic~tions th~t run in the VPC need to resolve  DNS requests to ~n on-premises ;;ctive  Directory dom~in th~t runs in the d~t~ center. Which solution will meet these requirements with the  LE;;ST ~dministr~tive overhe~d?
  ;;.  Provision ~ set of  EC2 inst~nces ~cross two ;;v~il~bility Zones in the VPC ~s c~ching  DNS servers to resolve  DNS queries from the ~pplic~tion servers within the VPC.
  B.  Provision ~n ;;m~zon  Route 53 priv~te hosted zone. Con gure  NS records th~t point to on-premises  DNS servers.
  C. Cre~te  DNS endpoints by using ;;m~zon  Route 53  Resolver. ;;dd condition~l forw~rding rules to resolve  DNS n~mesp~ces between the on- premises d~t~ center ~nd the VPC.
  D.  Provision ~ new ;;ctive  Directory dom~in controller in the VPC with ~ bidirection~l trust between this new dom~in ~nd the on-premises ;;ctive  Directory dom~in.

 Correct ;;nswer: C
 C (100%)

 Question #323
 ;; comp~ny processes environment~l d~t~. The comp~ny h~s set up sensors to provide ~ continuous stre~m of d~t~ from different ~re~s in ~ city. The d~t~ is ~v~il~ble in JSON form~t. The comp~ny w~nts to use ~n ;;WS solution to send the d~t~ to ~ d~t~b~se th~t does not require  xed schem~s for stor~ge. The d~t~ must be sent in re~l time. Which solution will meet these requirements?
  ;;. Use ;;m~zon  Kinesis  D~t~  Firehose to send the d~t~ to ;;m~zon  Redshift.
  B. Use ;;m~zon  Kinesis  D~t~ Stre~ms to send the d~t~ to ;;m~zon  Dyn~moDB.
  C. Use ;;m~zon  M~n~ged Stre~ming for ;;p~che  K~fk~ (;;m~zon  MSK) to send the d~t~ to ;;m~zon ;;uror~.
  D. Use ;;m~zon  Kinesis  D~t~  Firehose to send the d~t~ to ;;m~zon  Keysp~ces (for ;;p~che C~ss~ndr~).

 Correct ;;nswer: ;;
 B (100%)

 Question #324
 ;; comp~ny is migr~ting ~ leg~cy ~pplic~tion from ~n on-premises d~t~ center to ;;WS. The ~pplic~tion uses  MongoDB ~s ~ key-v~lue d~t~b~se. ;;ccording to the comp~ny's technic~l guidelines, ~ll ;;m~zon  EC2 inst~nces must be hosted in ~ priv~te subnet without ~n internet connection.  In ~ddition, ~ll connectivity between ~pplic~tions ~nd d~t~b~ses must be encrypted. The d~t~b~se must be ~ble to sc~le b~sed on dem~nd. Which solution will meet these requirements?
  ;;. Cre~te new ;;m~zon  DocumentDB (with  MongoDB comp~tibility) t~bles for the ~pplic~tion with  Provisioned  IOPS volumes. Use the inst~nce endpoint to connect to ;;m~zon  DocumentDB.
  B. Cre~te new ;;m~zon  Dyn~moDB t~bles for the ~pplic~tion with on-dem~nd c~p~city. Use ~ g~tew~y VPC endpoint for  Dyn~moDB to connect to the  Dyn~moDB t~bles.
  C. Cre~te new ;;m~zon  Dyn~moDB t~bles for the ~pplic~tion with on-dem~nd c~p~city. Use ~n interf~ce VPC endpoint for  Dyn~moDB to connect to the  Dyn~moDB t~bles.
  D. Cre~te new ;;m~zon  DocumentDB (with  MongoDB comp~tibility) t~bles for the ~pplic~tion with  Provisioned  IOPS volumes. Use the cluster endpoint to connect to ;;m~zon  DocumentDB.

 Correct ;;nswer: D
 B (53%)                               D (40%)              7%

 Question #325
 ;; comp~ny is running ~n ~pplic~tion on ;;m~zon  EC2 inst~nces in the ;;WS Cloud. The ~pplic~tion is using ~  MongoDB d~t~b~se with ~ replic~ set ~s its d~t~ tier. The  MongoDB d~t~b~se is inst~lled on systems in the comp~ny’s on-premises d~t~ center ~nd is ~ccessible through ~n ;;WS  Direct Connect connection to the d~t~ center environment. ;; solutions ~rchitect must migr~te the on-premises  MongoDB d~t~b~se to ;;m~zon  DocumentDB (with  MongoDB comp~tibility). Which str~tegy should the solutions ~rchitect choose to perform this migr~tion?
  ;;. Cre~te ~  eet of  EC2 inst~nces.  Inst~ll  MongoDB Community  Edition on the  EC2 inst~nces, ~nd cre~te ~ d~t~b~se. Con gure continuous synchronous replic~tion with the d~t~b~se th~t is running in the on-premises d~t~ center.
  B. Cre~te ~n ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) replic~tion inst~nce. Cre~te ~ source endpoint for the on-premises  MongoDB d~t~b~se by using ch~nge d~t~ c~pture (CDC). Cre~te ~ t~rget endpoint for the ;;m~zon  DocumentDB d~t~b~se. Cre~te ~nd run ~  DMS migr~tion t~sk.
  C. Cre~te ~ d~t~ migr~tion pipeline by using ;;WS  D~t~  Pipeline.  De ne d~t~ nodes for the on-premises  MongoDB d~t~b~se ~nd the ;;m~zon DocumentDB d~t~b~se. Cre~te ~ scheduled t~sk to run the d~t~ pipeline.
  D. Cre~te ~ source endpoint for the on-premises  MongoDB d~t~b~se by using ;;WS Glue cr~wlers. Con gure continuous ~synchronous replic~tion between the  MongoDB d~t~b~se ~nd the ;;m~zon  DocumentDB d~t~b~se.

 Correct ;;nswer: B
 B (100%)

 Question #326
 ;; comp~ny is re~rchitecting its ~pplic~tions to run on ;;WS. The comp~ny’s infr~structure includes multiple ;;m~zon  EC2 inst~nces. The comp~ny's development te~m needs different levels of ~ccess. The comp~ny w~nts to implement ~ policy th~t requires ~ll Windows  EC2 inst~nces to be joined to ~n ;;ctive  Directory dom~in on ;;WS. The comp~ny ~lso w~nts to implement enh~nced security processes such ~s multi- f~ctor ~uthentic~tion (MF;;). The comp~ny w~nts to use m~n~ged ;;WS services wherever possible. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;WS  Directory Service for  Microsoft ;;ctive  Directory implement~tion.  L~unch ~n ;;m~zon Worksp~ce. Connect to ~nd use the Worksp~ce for dom~in security con gur~tion t~sks.
  B. Cre~te ~n ;;WS  Directory Service for  Microsoft ;;ctive  Directory implement~tion.  L~unch ~n  EC2 inst~nce. Connect to ~nd use the  EC2 inst~nce for dom~in security con gur~tion t~sks.
  C. Cre~te ~n ;;WS  Directory Service Simple ;;D implement~tion.  L~unch ~n  EC2 inst~nce. Connect to ~nd use the  EC2 inst~nce for dom~in security con gur~tion t~sks.
  D. Cre~te ~n ;;WS  Directory Service Simple ;;D implement~tion.  L~unch ~n ;;m~zon Worksp~ce. Connect to ~nd use the Worksp~ce for dom~in security con gur~tion t~sks.

 Correct ;;nswer: ;;
 B (74%)                                  ;; (26%)

 Question #327
 ;; comp~ny w~nts to migr~te its on-premises ~pplic~tion to ;;WS. The d~t~b~se for the ~pplic~tion stores structured product d~t~ ~nd tempor~ry user session d~t~. The comp~ny needs to decouple the product d~t~ from the user session d~t~. The comp~ny ~lso needs to implement replic~tion in ~nother ;;WS  Region for dis~ster recovery. Which solution will meet these requirements with the  HIGHEST perform~nce?
  ;;. Cre~te ~n ;;m~zon  RDS  DB inst~nce with sep~r~te schem~s to host the product d~t~ ~nd the user session d~t~. Con gure ~ re~d replic~ for the  DB inst~nce in ~nother  Region.
  B. Cre~te ~n ;;m~zon  RDS  DB inst~nce to host the product d~t~. Con gure ~ re~d replic~ for the  DB inst~nce in ~nother  Region. Cre~te ~ glob~l d~t~store in ;;m~zon  El~stiC~che for  Memc~ched to host the user session d~t~.
  C. Cre~te two ;;m~zon  Dyn~moDB glob~l t~bles. Use one glob~l t~ble to host the product d~t~. Use the other glob~l t~ble to host the user session d~t~. Use  Dyn~moDB ;;cceler~tor (D;;X) for c~ching.
  D. Cre~te ~n ;;m~zon  RDS  DB inst~nce to host the product d~t~. Con gure ~ re~d replic~ for the  DB inst~nce in ~nother  Region. Cre~te ~n ;;m~zon  Dyn~moDB glob~l t~ble to host the user session d~t~.

 Correct ;;nswer: D
 D (46%)                        C (31%)                B (23%)

 Question #328
 ;; comp~ny orchestr~tes ~ multi-~ccount structure on ;;WS by using ;;WS Control Tower. The comp~ny is using ;;WS Org~niz~tions, ;;WS Con g, ~nd ;;WS Trusted ;;dvisor. The comp~ny h~s ~ speci c OU for development ~ccounts th~t developers use to experiment on ;;WS. The comp~ny h~s hundreds of developers, ~nd e~ch developer h~s ~n individu~l development ~ccount. The comp~ny w~nts to optimize costs in these development ~ccounts. ;;m~zon  EC2 inst~nces ~nd ;;m~zon  RDS inst~nces in these ~ccounts must be burst~ble. The comp~ny w~nts to dis~llow the use of other services th~t ~re not relev~nt. Wh~t should ~ solutions ~rchitect recommend to meet these requirements?
  ;;. Cre~te ~ custom SCP in ;;WS Org~niz~tions to ~llow the deployment of only burst~ble inst~nces ~nd to dis~llow services th~t ~re not relev~nt. ;;pply the SCP to the development OU.
  B. Cre~te ~ custom detective control (gu~rdr~il) in ;;WS Control Tower. Con gure the control (gu~rdr~il) to ~llow the deployment of only burst~ble inst~nces ~nd to dis~llow services th~t ~re not relev~nt. ;;pply the control (gu~rdr~il) to the development OU.
  C. Cre~te ~ custom preventive control (gu~rdr~il) in ;;WS Control Tower. Con gure the control (gu~rdr~il) to ~llow the deployment of only burst~ble inst~nces ~nd to dis~llow services th~t ~re not relev~nt. ;;pply the control (gu~rdr~il) to the development OU.
  D. Cre~te ~n ;;WS Con g rule in the ;;WS Control Tower ~ccount. Con gure the ;;WS Con g rule to ~llow the deployment of only burst~ble inst~nces ~nd to dis~llow services th~t ~re not relev~nt.  Deploy the ;;WS Con g rule to the development OU by using ;;WS CloudForm~tion St~ckSets.

 Correct ;;nswer: ;;
 C (82%)                                 ;; (18%)

 Question #329
 ;;  n~nci~l services comp~ny runs ~ complex, multi-tier ~pplic~tion on ;;m~zon  EC2 inst~nces ~nd ;;WS  L~mbd~ functions. The ~pplic~tion stores tempor~ry d~t~ in ;;m~zon S3. The S3 objects ~re v~lid for only 45 minutes ~nd ~re deleted ~fter 24 hours. The comp~ny deploys e~ch version of the ~pplic~tion by l~unching ~n ;;WS CloudForm~tion st~ck. The st~ck cre~tes ~ll resources th~t ~re required to run the ~pplic~tion. When the comp~ny deploys ~nd v~lid~tes ~ new ~pplic~tion version, the comp~ny deletes the CloudForm~tion st~ck of the old version. The comp~ny recently tried to delete the CloudForm~tion st~ck of ~n old ~pplic~tion version, but the oper~tion f~iled. ;;n ~n~lysis shows th~t CloudForm~tion f~iled to delete ~n existing S3 bucket. ;; solutions ~rchitect needs to resolve this issue without m~king m~jor ch~nges to the ~pplic~tion's ~rchitecture. Which solution meets these requirements?
  ;;.  Implement ~  L~mbd~ function th~t deletes ~ll  les from ~ given S3 bucket.  Integr~te this  L~mbd~ function ~s ~ custom resource into the CloudForm~tion st~ck.  Ensure th~t the custom resource h~s ~  DependsOn ~ttribute th~t points to the S3 bucket's resource.
  B.  Modify the CloudForm~tion templ~te to provision ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system to store the tempor~ry  les there inste~d of in ;;m~zon S3. Con gure the  L~mbd~ functions to run in the s~me VPC ~s the  le system.  Mount the  le system to the  EC2 inst~nces ~nd  L~mbd~ functions.
  C.  Modify the CloudF orm~tion st~ck to cre~te ~n S3  Lifecycle rule th~t expires ~ll objects 45 minutes ~fter cre~tion. ;;dd ~  DependsOn ~ttribute th~t points to the S3 bucket’s resource.
  D.  Modify the CloudForm~tion st~ck to ~tt~ch ~  DeletionPolicy ~ttribute with ~ v~lue of  Delete to the S3 bucket.

 Correct ;;nswer: B
 ;; (88%)                                    13%

 Question #330
 ;; comp~ny h~s developed ~ mobile g~me. The b~ckend for the g~me runs on sever~l virtu~l m~chines loc~ted in ~n on-premises d~t~ center. The business logic is exposed using ~  REST ;;PI with multiple functions.  Pl~yer session d~t~ is stored in centr~l  le stor~ge.  B~ckend services use different ;;PI keys for throttling ~nd to distinguish between live ~nd test tr~ c. The lo~d on the g~me b~ckend v~ries throughout the d~y.  During pe~k hours, the server c~p~city is not su cient. There ~re ~lso l~tency issues when fetching pl~yer session d~t~.  M~n~gement h~s ~sked ~ solutions ~rchitect to present ~ cloud ~rchitecture th~t c~n h~ndle the g~me’s v~rying lo~d ~nd provide low-l~tency d~t~ ~ccess. The ;;PI model should not be ch~nged. Which solution meets these requirements?
  ;;.  Implement the  REST ;;PI using ~  Network  Lo~d  B~l~ncer (NLB).  Run the business logic on ~n ;;m~zon  EC2 inst~nce behind the  NLB. Store pl~yer session d~t~ in ;;m~zon ;;uror~ Serverless.
  B.  Implement the  REST ;;PI using ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB).  Run the business logic in ;;WS  L~mbd~. Store pl~yer session d~t~ in ;;m~zon  Dyn~moDB with on-dem~nd c~p~city.
  C.  Implement the  REST ;;PI using ;;m~zon ;;PI G~tew~y.  Run the business logic in ;;WS  L~mbd~. Store pl~yer session d~t~ in ;;m~zon Dyn~moDB with on-dem~nd c~p~city.
  D.  Implement the  REST ;;PI using ;;WS ;;ppSync.  Run the business logic in ;;WS  L~mbd~. Store pl~yer session d~t~ in ;;m~zon ;;uror~ Serverless.

 Correct ;;nswer: D
 C (100%)

 Question #331
 ;; comp~ny is migr~ting ~n ~pplic~tion to the ;;WS Cloud. The ~pplic~tion runs in ~n on-premises d~t~ center ~nd writes thous~nds of im~ges into ~ mounted  NFS  le system e~ch night. ;;fter the comp~ny migr~tes the ~pplic~tion, the comp~ny will host the ~pplic~tion on ~n ;;m~zon  EC2 inst~nce with ~ mounted ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system. The comp~ny h~s est~blished ~n ;;WS  Direct Connect connection to ;;WS.  Before the migr~tion cutover, ~ solutions ~rchitect must build ~ process th~t will replic~te the newly cre~ted on-premises im~ges to the  EFS  le system. Wh~t is the  MOST oper~tion~lly e cient w~y to replic~te the im~ges?
  ;;. Con gure ~ periodic process to run the ~ws s3 sync comm~nd from the on-premises  le system to ;;m~zon S3. Con gure ~n ;;WS  L~mbd~ function to process event noti c~tions from ;;m~zon S3 ~nd copy the im~ges from ;;m~zon S3 to the  EFS  le system.
  B.  Deploy ~n ;;WS Stor~ge G~tew~y  le g~tew~y with ~n  NFS mount point.  Mount the  le g~tew~y  le system on the on-premises server. Con gure ~ process to periodic~lly copy the im~ges to the mount point.
  C.  Deploy ~n ;;WS  D~t~Sync ~gent to ~n on-premises server th~t h~s ~ccess to the  NFS  le system. Send d~t~ over the  Direct Connect connection to ~n S3 bucket by using ~ public VIF. Con gure ~n ;;WS  L~mbd~ function to process event noti c~tions from ;;m~zon S3 ~nd copy the im~ges from ;;m~zon S3 to the  EFS  le system.
  D.  Deploy ~n ;;WS  D~t~Sync ~gent to ~n on-premises server th~t h~s ~ccess to the  NFS  le system. Send d~t~ over the  Direct Connect connection to ~n ;;WS  Priv~teLink interf~ce VPC endpoint for ;;m~zon  EFS by using ~ priv~te VIF. Con gure ~  D~t~Sync scheduled t~sk to send the im~ges to the  EFS  le system every 24 hours.

 Correct ;;nswer: C
 D (100%)

 Question #332
 ;; comp~ny recently migr~ted ~ web ~pplic~tion from ~n on-premises d~t~ center to the ;;WS Cloud. The web ~pplic~tion infr~structure consists of ~n ;;m~zon CloudFront distribution th~t routes to ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB), with ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) to process requests. ;; recent security ~udit reve~led th~t the web ~pplic~tion is ~ccessible by using both CloudFront ~nd ;;LB endpoints.  However, the comp~ny requires th~t the web ~pplic~tion must be ~ccessible only by using the CloudFront endpoint. Which solution will meet this requirement with the  LE;;ST ~mount of effort?
  ;;. Cre~te ~ new security group ~nd ~tt~ch it to the CloudFront distribution. Upd~te the ;;LB security group ingress to ~llow ~ccess only from the CloudFront security group.
  B. Upd~te ;;LB security group ingress to ~llow ~ccess only from the com.~m~zon~ws.glob~l.cloudfront.origin-f~cing CloudFront m~n~ged pre x list.
  C. Cre~te ~ com.~m~zon~ws.region.el~sticlo~db~l~ncing VPC interf~ce endpoint for  El~stic  Lo~d  B~l~ncing. Upd~te the ;;LB scheme from internet-f~cing to intern~l.
  D.  Extr~ct CloudFront  IPs from the ;;WS provided ip-r~nges.json document. Upd~te ;;LB security group ingress to ~llow ~ccess only from CloudFront  IPs.

 Correct ;;nswer: ;;
 B (100%)

 Question #333
 ;; comp~ny hosts ~ community forum site using ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd ~  Docker ~pplic~tion hosted in ~n ;;m~zon  ECS cluster. The site d~t~ is stored in ;;m~zon  RDS for  MySQL ~nd the cont~iner im~ge is stored in  ECR. The comp~ny needs to provide their customers with ~ dis~ster recovery SL;; with ~n  RTO of no more th~n 24 hours ~nd  RPO of no more th~n 8 hours. Which of the following solutions is the  MOST cost-effective w~y to meet the requirements?
  ;;. Use ;;WS CloudForm~tion to deploy identic~l ;;LB,  EC2,  ECS ~nd  RDS resources in two regions. Schedule  RDS sn~pshots every 8 hours. Use RDS multi-region replic~tion to upd~te the second~ry region's copy of the d~t~b~se.  In the event of ~ f~ilure, restore from the l~test sn~pshot, ~nd use ~n ;;m~zon  Route 53  DNS f~ilover policy to ~utom~tic~lly redirect customers to the ;;LB in the second~ry region.
  B. Store the  Docker im~ge in  ECR in two regions. Schedule  RDS sn~pshots every 8 hours with sn~pshots copied to the second~ry region.  In the event of ~ f~ilure, use ;;WS CloudForm~tion to deploy the ;;LB,  EC2,  ECS ~nd  RDS resources in the second~ry region, restore from the l~test sn~pshot, ~nd upd~te the  DNS record to point to the ;;LB in the second~ry region.
  C. Use ;;WS CloudForm~tion to deploy identic~l ;;LB,  EC2,  ECS, ~nd  RDS resources in ~ second~ry region. Schedule hourly  RDS  MySQL b~ckups to ;;m~zon S3 ~nd use cross-region replic~tion to replic~te d~t~ to ~ bucket in the second~ry region.  In the event of ~ f~ilure, import the l~test  Docker im~ge to ;;m~zon  ECR in the second~ry region, deploy to the  EC2 inst~nce, restore the l~test  MySQL b~ckup, ~nd upd~te the DNS record to point to the ;;LB in the second~ry region.
  D.  Deploy ~ pilot light environment in ~ second~ry region with ~n ;;LB ~nd ~ minim~l resource  EC2 deployment for  Docker in ~n ;;WS ;;uto Sc~ling group with ~ sc~ling policy to incre~se inst~nce size ~nd number of nodes. Cre~te ~ cross-region re~d replic~ of the  RDS d~t~.  In the event of ~ f~ilure, promote the replic~ to prim~ry, ~nd upd~te the  DNS record to point to the ;;LB in the second~ry region.

 Correct ;;nswer: B
 B (89%)                                    11%

 Question #334
 ;; comp~ny is migr~ting its infr~structure to the ;;WS Cloud. The comp~ny must comply with ~ v~riety of regul~tory st~nd~rds for different projects. The comp~ny needs ~ multi-~ccount environment. ;; solutions ~rchitect needs to prep~re the b~seline infr~structure. The solution must provide ~ consistent b~seline of m~n~gement ~nd security, but it must ~llow  exibility for different compli~nce requirements within v~rious ;;WS ~ccounts. The solution ~lso needs to integr~te with the existing on-premises ;;ctive  Directory  Feder~tion Services (;;D  FS) server. Which solution meets these requirements with the  LE;;ST ~mount of oper~tion~l overhe~d?
  ;;. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Cre~te ~ single SCP for le~st privilege ~ccess ~cross ~ll ~ccounts. Cre~te ~ single OU for ~ll ~ccounts. Con gure ~n  I;;M identity provider for feder~tion with the on-premises ;;D  FS server. Con gure ~ centr~l logging ~ccount with ~ de ned process for log gener~ting services to send log events to the centr~l ~ccount.  En~ble ;;WS Con g in the centr~l ~ccount with conform~nce p~cks for ~ll ~ccounts.
  B. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions.  En~ble ;;WS Control Tower on the org~niz~tion.  Review included controls (gu~rdr~ils) for SCPs. Check ;;WS Con g for ~re~s th~t require ~dditions. ;;dd OUs ~s necess~ry. Connect ;;WS  I;;M  Identity Center (;;WS Single Sign-On) to the on-premises ;;D  FS server.
  C. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Cre~te SCPs for le~st privilege ~ccess. Cre~te ~n OU structure, ~nd use it to group ;;WS ~ccounts. Connect ;;WS  I;;M  Identity Center (;;WS Single Sign-On) to the on-premises ;;D  FS server. Con gure ~ centr~l logging ~ccount with ~ de ned process for log gener~ting services to send log events to the centr~l ~ccount.  En~ble ;;WS Con g in the centr~l ~ccount with ~ggreg~tors ~nd conform~nce p~cks.
  D. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions.  En~ble ;;WS Control Tower on the org~niz~tion.  Review included controls (gu~rdr~ils) for SCPs. Check ;;WS Con g for ~re~s th~t require ~dditions. Con gure ~n  I;;M identity provider for feder~tion with the on-premises ;;D  FS server.

 Correct ;;nswer: D
 B (100%)

 Question #335
 ;;n online m~g~zine will l~unch its l~test edition this month. This edition will be the  rst to be distributed glob~lly. The m~g~zine's dyn~mic website currently uses ~n ;;pplic~tion  Lo~d  B~l~ncer in front of the web tier, ~  eet of ;;m~zon  EC2 inst~nces for web ~nd ~pplic~tion servers, ~nd ;;m~zon ;;uror~  MySQL.  Portions of the website include st~tic content ~nd ~lmost ~ll tr~ c is re~d-only. The m~g~zine is expecting ~ signi c~nt spike in internet tr~ c when the new edition is l~unched. Optim~l perform~nce is ~ top priority for the week following the l~unch. Which combin~tion of steps should ~ solutions ~rchitect t~ke to reduce system response times for ~ glob~l ~udience? (Choose two.)
  ;;. Use logic~l cross-Region replic~tion to replic~te the ;;uror~  MySQL d~t~b~se to ~ second~ry  Region.  Repl~ce the web servers with ;;m~zon S3.  Deploy S3 buckets in cross-Region replic~tion mode.
  B.  Ensure the web ~nd ~pplic~tion tiers ~re e~ch in ;;uto Sc~ling groups.  Introduce ~n ;;WS  Direct Connect connection.  Deploy the web ~nd ~pplic~tion tiers in  Regions ~cross the world.
  C.  Migr~te the d~t~b~se from ;;m~zon ;;uror~ to ;;m~zon  RDS for  MySQL.  Ensure ~ll three of the ~pplic~tion tiers  – web, ~pplic~tion, ~nd d~t~b~se  – ~re in priv~te subnets.
  D. Use ~n ;;uror~ glob~l d~t~b~se for physic~l cross-Region replic~tion. Use ;;m~zon S3 with cross-Region replic~tion for st~tic content ~nd resources.  Deploy the web ~nd ~pplic~tion tiers in  Regions ~cross the world.
  E.  Introduce ;;m~zon  Route 53 with l~tency-b~sed routing ~nd ;;m~zon CloudFront distributions.  Ensure the web ~nd ~pplic~tion tiers ~re e~ch in ;;uto Sc~ling groups.

 Correct ;;nswer: DE
 DE (100%)

 Question #336
 ;;n online g~ming comp~ny needs to optimize the cost of its worklo~ds on ;;WS. The comp~ny uses ~ dedic~ted ~ccount to host the production environment for its online g~ming ~pplic~tion ~nd ~n ~n~lytics ~pplic~tion. ;;m~zon  EC2 inst~nces host the g~ming ~pplic~tion ~nd must ~lw~ys be ~v~il~ble. The  EC2 inst~nces run ~ll ye~r. The ~n~lytics ~pplic~tion uses d~t~ th~t is stored in ;;m~zon S3. The ~n~lytics ~pplic~tion c~n be interrupted ~nd resumed without issue. Which solution will meet these requirements  MOST cost-effectively?
  ;;.  Purch~se ~n  EC2  Inst~nce S~vings  Pl~n for the online g~ming ~pplic~tion inst~nces. Use On-Dem~nd  Inst~nces for the ~n~lytics ~pplic~tion.
  B.  Purch~se ~n  EC2  Inst~nce S~vings  Pl~n for the online g~ming ~pplic~tion inst~nces. Use Spot  Inst~nces for the ~n~lytics ~pplic~tion.
  C. Use Spot  Inst~nces for the online g~ming ~pplic~tion ~nd the ~n~lytics ~pplic~tion. Set up ~ c~t~log in ;;WS Service C~t~log to provision services ~t ~ discount.
  D. Use On-Dem~nd  Inst~nces for the online g~ming ~pplic~tion. Use Spot  Inst~nces for the ~n~lytics ~pplic~tion. Set up ~ c~t~log in ;;WS Service C~t~log to provision services ~t ~ discount.

 Correct ;;nswer: B
 B (100%)

 Question #337
 ;; comp~ny runs ~pplic~tions in hundreds of production ;;WS ~ccounts. The comp~ny uses ;;WS Org~niz~tions with ~ll fe~tures en~bled ~nd h~s ~ centr~lized b~ckup oper~tion th~t uses ;;WS  B~ckup. The comp~ny is concerned ~bout r~nsomw~re ~tt~cks. To ~ddress this concern, the comp~ny h~s cre~ted ~ new policy th~t ~ll b~ckups must be resilient to bre~ches of privileged-user credenti~ls in ~ny production ~ccount. Which combin~tion of steps will meet this new requirement? (Choose three.)
  ;;.  Implement cross-~ccount b~ckup with ;;WS  B~ckup v~ults in design~ted non-production ~ccounts.
  B. ;;dd ~n SCP th~t restricts the modi c~tion of ;;WS  B~ckup v~ults.
  C.  Implement ;;WS  B~ckup V~ult  Lock in compli~nce mode.
  C.  Implement le~st privilege ~ccess for the  I;;M service role th~t is ~ssigned to ;;WS  B~ckup.
  D. Con gure the b~ckup frequency, lifecycle, ~nd retention period to ensure th~t ~t le~st one b~ckup ~lw~ys exists in the cold tier.
  E. Con gure ;;WS  B~ckup to write ~ll b~ckups to ~n ;;m~zon S3 bucket in ~ design~ted non-production ~ccount.  Ensure th~t the S3 bucket h~s S3 Object  Lock en~bled.

 Correct ;;nswer: ;;CD
 ;;CD (39%)                     ;;CE (33%)                ;;BC (28%)

 Question #338
 ;; comp~ny needs to ~ggreg~te ;;m~zon CloudW~tch logs from its ;;WS ~ccounts into one centr~l logging ~ccount. The collected logs must rem~in in the ;;WS  Region of cre~tion. The centr~l logging ~ccount will then process the logs, norm~lize the logs into st~nd~rd output form~t, ~nd stre~m the output logs to ~ security tool for more processing. ;; solutions ~rchitect must design ~ solution th~t c~n h~ndle ~ l~rge volume of logging d~t~ th~t needs to be ingested.  Less logging will occur outside norm~l business hours th~n during norm~l business hours. The logging solution must sc~le with the ~nticip~ted lo~d. The solutions ~rchitect h~s decided to use ~n ;;WS Control Tower design to h~ndle the multi-~ccount logging process. Which combin~tion of steps should the solutions ~rchitect t~ke to meet the requirements? (Choose three.)
  ;;. Cre~te ~ destin~tion ;;m~zon  Kinesis d~t~ stre~m in the centr~l logging ~ccount.
  B. Cre~te ~ destin~tion ;;m~zon Simple Queue Service (;;m~zon SQS) queue in the centr~l logging ~ccount.
  C. Cre~te ~n  I;;M role th~t gr~nts ;;m~zon CloudW~tch  Logs the permission to ~dd d~t~ to the ;;m~zon  Kinesis d~t~ stre~m. Cre~te ~ trust policy. Specify the trust policy in the  I;;M role.  In e~ch member ~ccount, cre~te ~ subscription  lter for e~ch log group to send d~t~ to the Kinesis d~t~ stre~m.
  D. Cre~te ~n  I;;M role th~t gr~nts ;;m~zon CloudW~tch  Logs the permission to ~dd d~t~ to the ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Cre~te ~ trust policy. Specify the trust policy in the  I;;M role.  In e~ch member ~ccount, cre~te ~ single subscription  lter for ~ll log groups to send d~t~ to the SQS queue.
  E. Cre~te ~n ;;WS  L~mbd~ function.  Progr~m the  L~mbd~ function to norm~lize the logs in the centr~l logging ~ccount ~nd to write the logs to the security tool.
  F. Cre~te ~n ;;WS  L~mbd~ function.  Progr~m the  L~mbd~ function to norm~lize the logs in the member ~ccounts ~nd to write the logs to the security tool.

 Correct ;;nswer: BFD
 ;;CE (100%)

 Question #339
 ;; comp~ny is migr~ting ~ leg~cy ~pplic~tion from ~n on-premises d~t~ center to ;;WS. The ~pplic~tion consists of ~ single ~pplic~tion server ~nd ~  Microsoft SQL Server d~t~b~se server.  E~ch server is deployed on ~ VMw~re VM th~t consumes 500 TB of d~t~ ~cross multiple ~tt~ched volumes. The comp~ny h~s est~blished ~  10 Gbps ;;WS  Direct Connect connection from the closest ;;WS  Region to its on-premises d~t~ center. The  Direct Connect connection is not currently in use by other services. Which combin~tion of steps should ~ solutions ~rchitect t~ke to migr~te the ~pplic~tion with the  LE;;ST ~mount of downtime? (Choose two.)
  ;;. Use ~n ;;WS Server  Migr~tion Service (;;WS SMS) replic~tion job to migr~te the d~t~b~se server VM to ;;WS.
  B. Use VM  Import/Export to import the ~pplic~tion server VM.
  C.  Export the VM im~ges to ~n ;;WS Snowb~ll  Edge Stor~ge Optimized device.
  D. Use ~n ;;WS Server  Migr~tion Service (;;WS SMS) replic~tion job to migr~te the ~pplic~tion server VM to ;;WS.
  E. Use ~n ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) replic~tion inst~nce to migr~te the d~t~b~se to ~n ;;m~zon  RDS  DB inst~nce.

 Correct ;;nswer: ;;D
 DE (43%)                        ;;D (36%)               BE (21%)

 Question #340
 ;; comp~ny oper~tes ~  eet of servers on premises ~nd oper~tes ~  eet of ;;m~zon  EC2 inst~nces in its org~niz~tion in ;;WS Org~niz~tions. The comp~ny's ;;WS ~ccounts cont~in hundreds of VPCs. The comp~ny w~nts to connect its ;;WS ~ccounts to its on-premises network. ;;WS Site-to- Site VPN connections ~re ~lre~dy est~blished to ~ single ;;WS ~ccount. The comp~ny w~nts to control which VPCs c~n communic~te with other VPCs. Which combin~tion of steps will ~chieve this level of control with the  LE;;ST oper~tion~l effort? (Choose three.)
  ;;. Cre~te ~ tr~nsit g~tew~y in ~n ;;WS ~ccount. Sh~re the tr~nsit g~tew~y ~cross ~ccounts by using ;;WS  Resource ;;ccess  M~n~ger (;;WS R;;M).
  B. Con gure ~tt~chments to ~ll VPCs ~nd VPNs.
  C. Setup tr~nsit g~tew~y route t~bles. ;;ssoci~te the VPCs ~nd VPNs with the route t~bles.
  D. Con gure VPC peering between the VPCs.
  E. Con gure ~tt~chments between the VPCs ~nd VPNs.
  F. Setup route t~bles on the VPCs ~nd VPNs.

 Correct ;;nswer: FDC
 ;;BC (55%)                               ;;CE (45%)

 Question #341
 ;; comp~ny needs to optimize the cost of its ~pplic~tion on ;;WS. The ~pplic~tion uses ;;WS  L~mbd~ functions ~nd ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cont~iners th~t run on ;;WS  F~rg~te. The ~pplic~tion is write-he~vy ~nd stores d~t~ in ~n ;;m~zon ;;uror~  MySQL d~t~b~se. The lo~d on the ~pplic~tion is not consistent. The ~pplic~tion experiences long periods of no us~ge, followed by sudden ~nd signi c~nt incre~ses ~nd decre~ses in tr~ c. The d~t~b~se runs on ~ memory optimized  DB inst~nce th~t c~nnot h~ndle the lo~d. ;; solutions ~rchitect must design ~ solution th~t c~n sc~le to h~ndle the ch~nges in tr~ c. Which solution will meet these requirements  MOST cost-effectively?
  ;;. ;;dd ~ddition~l re~d replic~s to the d~t~b~se.  Purch~se  Inst~nce S~vings  Pl~ns ~nd  RDS  Reserved  Inst~nces.
  B.  Migr~te the d~t~b~se to ~n ;;uror~  DB cluster th~t h~s multiple writer inst~nces.  Purch~se  Inst~nce S~vings  Pl~ns.
  C.  Migr~te the d~t~b~se to ~n ;;uror~ glob~l d~t~b~se.  Purch~se Compute S~vings  Pl~ns ~nd  RDS  Reserved inst~nces.
  D.  Migr~te the d~t~b~se to ;;uror~ Serverless v1.  Purch~se Compute S~vings  Pl~ns.

 Correct ;;nswer: B
 D (100%)

 Question #342
 ;; comp~ny migr~ted ~n ~pplic~tion to the ;;WS Cloud. The ~pplic~tion runs on two ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). ;;pplic~tion d~t~ is stored in ~  MySQL d~t~b~se th~t runs on ~n ~ddition~l  EC2 inst~nce. The ~pplic~tion's use of the d~t~b~se is re~d-he~vy. The ~pplic~tion lo~ds st~tic content from ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes th~t ~re ~tt~ched to e~ch  EC2 inst~nce. The st~tic content is upd~ted frequently ~nd must be copied to e~ch  EBS volume. The lo~d on the ~pplic~tion ch~nges throughout the d~y.  During pe~k hours, the ~pplic~tion c~nnot h~ndle ~ll the incoming requests. Tr~ce d~t~ shows th~t the d~t~b~se c~nnot h~ndle the re~d lo~d during pe~k hours. Which solution will improve the reli~bility of the ~pplic~tion?
  ;;.  Migr~te the ~pplic~tion to ~ set of ;;WS  L~mbd~ functions. Set the  L~mbd~ functions ~s t~rgets for the ;;LB. Cre~te ~ new single  EBS volume for the st~tic content. Con gure the  L~mbd~ functions to re~d from the new  EBS volume.  Migr~te the d~t~b~se to ~n ;;m~zon  RDS for MySQL  Multi-;;Z  DB cluster.
  B.  Migr~te the ~pplic~tion to ~ set of ;;WS Step  Functions st~te m~chines. Set the st~te m~chines ~s t~rgets for the ;;LCre~te ~n ;;m~zon El~stic  File System (;;m~zon  EFS)  le system for the st~tic content. Con gure the st~te m~chines to re~d from the  EFS  le system.  Migr~te the d~t~b~se to ;;m~zon ;;uror~  MySQL Serverless v2 with ~ re~der  DB inst~nce.
  C. Cont~inerize the ~pplic~tion.  Migr~te the ~pplic~tion to ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster. Use the ;;WS  F~rg~te l~unch type for the t~sks th~t host the ~pplic~tion. Cre~te ~ new single  EBS volume for the st~tic content.  Mount the new  EBS volume on the ECS cluster. Con gure ;;WS ;;pplic~tion ;;uto Sc~ling on the  ECS cluster. Set the  ECS service ~s ~ t~rget for the ;;LB.  Migr~te the d~t~b~se to ~n ;;m~zon  RDS for  MySQL  Multi-;;Z  DB cluster.
  D. Cont~inerize the ~pplic~tion.  Migr~te the ~pplic~tion to ~n ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) cluster. Use the ;;WS  F~rg~te l~unch type for the t~sks th~t host the ~pplic~tion. Cre~te ~n ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system for the st~tic content. Mount the  EFS  le system to e~ch cont~iner. Con gure ;;WS ;;pplic~tion ;;uto Sc~ling on the  ECS cluster. Set the  ECS service ~s ~ t~rget for the ;;LB.  Migr~te the d~t~b~se to ;;m~zon ;;uror~  MySQL Serverless v2 with ~ re~der  DB inst~nce.

 Correct ;;nswer: B
 D (87%)                                    13%

 Question #343
 ;; solutions ~rchitect w~nts to m~ke sure th~t only ;;WS users or roles with suit~ble permissions c~n ~ccess ~ new ;;m~zon ;;PI G~tew~y endpoint. The solutions ~rchitect w~nts ~n end-to-end view of e~ch request to ~n~lyze the l~tency of the request ~nd cre~te service m~ps. How c~n the solutions ~rchitect design the ;;PI G~tew~y ~ccess control ~nd perform request inspections?
  ;;.  For the ;;PI G~tew~y method, set the ~uthoriz~tion to ;;WS_I;;M. Then, give the  I;;M user or role execute-~pi:Invoke permission on the  REST ;;PI resource.  En~ble the ;;PI c~ller to sign requests with ;;WS Sign~ture when ~ccessing the endpoint. Use ;;WS X-R~y to tr~ce ~nd ~n~lyze user requests to ;;PI G~tew~y.
  B.  For the ;;PI G~tew~y resource, set CORS to en~bled ~nd only return the comp~ny's dom~in in ;;ccess-Control-;;llow-Origin he~ders. Then, give the  I;;M user or role execute-~pi:Invoke permission on the  REST ;;PI resource. Use ;;m~zon CloudW~tch to tr~ce ~nd ~n~lyze user requests to ;;PI G~tew~y.
  C. Cre~te ~n ;;WS  L~mbd~ function ~s the custom ~uthorizer, ~sk the ;;PI client to p~ss the key ~nd secret when m~king the c~ll, ~nd then use L~mbd~ to v~lid~te the key/secret p~ir ~g~inst the  I;;M system. Use ;;WS X-R~y to tr~ce ~nd ~n~lyze user requests to ;;PI G~tew~y.
  D. Cre~te ~ client certi c~te for ;;PI G~tew~y.  Distribute the certi c~te to the ;;WS users ~nd roles th~t need to ~ccess the endpoint.  En~ble the ;;PI c~ller to p~ss the client certi c~te when ~ccessing the endpoint. Use ;;m~zon CloudW~tch to tr~ce ~nd ~n~lyze user requests to ;;PI G~tew~y.

 Correct ;;nswer: ;;
 ;; (100%)

 Question #344
 ;; comp~ny is using ;;WS CodePipeline for the CI/CD of ~n ~pplic~tion to ~n ;;m~zon  EC2 ;;uto Sc~ling group. ;;ll ;;WS resources ~re de ned in ;;WS CloudForm~tion templ~tes. The ~pplic~tion ~rtif~cts ~re stored in ~n ;;m~zon S3 bucket ~nd deployed to the ;;uto Sc~ling group using inst~nce user d~t~ scripts. ;;s the ~pplic~tion h~s become more complex, recent resource ch~nges in the CloudForm~tion templ~tes h~ve c~used unpl~nned downtime. How should ~ solutions ~rchitect improve the CI/CD pipeline to reduce the likelihood th~t ch~nges in the templ~tes will c~use downtime?
  ;;. ;;d~pt the deployment scripts to detect ~nd report CloudForm~tion error conditions when performing deployments. Write test pl~ns for ~ testing te~m to run in ~ non-production environment before ~pproving the ch~nge for production.
  B.  Implement ~utom~ted testing using ;;WS CodeBuild in ~ test environment. Use CloudForm~tion ch~nge sets to ev~lu~te ch~nges before deployment. Use ;;WS CodeDeploy to lever~ge blue/green deployment p~tterns to ~llow ev~lu~tions ~nd the ~bility to revert ch~nges, if needed.
  C. Use plugins for the integr~ted development environment (IDE) to check the templ~tes for errors, ~nd use the ;;WS CLI to v~lid~te th~t the templ~tes ~re correct. ;;d~pt the deployment code to check for error conditions ~nd gener~te noti c~tions on errors.  Deploy to ~ test environment ~nd run ~ m~nu~l test pl~n before ~pproving the ch~nge for production.
  D. Use ;;WS CodeDeploy ~nd ~ blue/green deployment p~ttern with CloudForm~tion to repl~ce the user d~t~ deployment scripts.  H~ve the oper~tors log in to running inst~nces ~nd go through ~ m~nu~l test pl~n to verify the ~pplic~tion is running ~s expected.

 Correct ;;nswer: D
 B (100%)

 Question #345
 ;;  North ;;meric~n comp~ny with he~dqu~rters on the  E~st Co~st is deploying ~ new web ~pplic~tion running on ;;m~zon  EC2 in the us-e~st-1 Region. The ~pplic~tion should dyn~mic~lly sc~le to meet user dem~nd ~nd m~int~in resiliency. ;;ddition~lly, the ~pplic~tion must h~ve dis~ster recovery c~p~bilities in ~n ~ctive-p~ssive con gur~tion with the us-west-1  Region. Which steps should ~ solutions ~rchitect t~ke ~fter cre~ting ~ VPC in the us-e~st-1  Region?
  ;;. Cre~te ~ VPC in the us-west-1  Region. Use inter-Region VPC peering to connect both VPCs.  Deploy ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) sp~nning multiple ;;v~il~bility Zones (;;Zs) to the VPC in the us-e~st-1  Region.  Deploy  EC2 inst~nces ~cross multiple ;;Zs in e~ch  Region ~s p~rt of ~n ;;uto Sc~ling group sp~nning both VPCs ~nd served by the ;;LB.
  B.  Deploy ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) sp~nning multiple ;;v~il~bility Zones (;;Zs) to the VPC in the us-e~st-1  Region.  Deploy  EC2 inst~nces ~cross multiple ;;Zs ~s p~rt of ~n ;;uto Sc~ling group served by the ;;LDeploy the s~me solution to the us-west-1  Region. Cre~te ~n ;;m~zon  Route 53 record set with ~ f~ilover routing policy ~nd he~lth checks en~bled to provide high ~v~il~bility ~cross both  Regions.
  C. Cre~te ~ VPC in the us-west-1  Region. Use inter-Region VPC peering to connect both VPCs.  Deploy ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) th~t sp~ns both VPCs.  Deploy  EC2 inst~nces ~cross multiple ;;v~il~bility Zones ~s p~rt of ~n ;;uto Sc~ling group in e~ch VPC served by the ;;LB. Cre~te ~n ;;m~zon  Route 53 record th~t points to the ;;LB.
  D.  Deploy ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) sp~nning multiple ;;v~il~bility Zones (;;Zs) to the VPC in the us-e~st-1  Region.  Deploy  EC2 inst~nces ~cross multiple ;;Zs ~s p~rt of ~n ;;uto Sc~ling group served by the ;;LB.  Deploy the s~me solution to the us-west-1  Region. Cre~te sep~r~te ;;m~zon  Route 53 records in e~ch  Region th~t point to the ;;LB in the  Region. Use  Route 53 he~lth checks to provide high ~v~il~bility ~cross both  Regions.

 Correct ;;nswer: ;;
 B (100%)

 Question #346
 ;; comp~ny h~s ~ leg~cy ~pplic~tion th~t runs on multiple  NET  Fr~mework components. The components sh~re the s~me  Microsoft SQL Server d~t~b~se ~nd communic~te with e~ch other ~synchronously by using  Microsoft  Mess~ge Queueing (MSMQ). The comp~ny is st~rting ~ migr~tion to cont~inerized .NET Core components ~nd w~nts to ref~ctor the ~pplic~tion to run on ;;WS. The .NET Core components require complex orchestr~tion. The comp~ny must h~ve full control over networking ~nd host con gur~tion. The ~pplic~tion's d~t~b~se model is strongly rel~tion~l. Which solution will meet these requirements?
  ;;.  Host the  INET Core components on ;;WS ;;pp  Runner.  Host the d~t~b~se on ;;m~zon  RDS for SQL Server. Use ;;m~zon  EventBiridge for ~synchronous mess~ging.
  B.  Host the .NET Core components on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the ;;WS  F~rg~te l~unch type.  Host the d~t~b~se on ;;m~zon  Dyn~moDUse ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) for ~synchronous mess~ging.
  C.  Host the .NET Core components on ;;WS  El~stic  Be~nst~lk.  Host the d~t~b~se on ;;m~zon ;;uror~  PostgreSQL Serverless v2. Use ;;m~zon M~n~ged Stre~ming for ;;p~che  K~fk~ (;;m~zon  MSK) for ~synchronous mess~ging.
  D.  Host the  NET Core components on ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) with the ;;m~zon  EC2 l~unch type.  Host the d~t~b~se on ;;m~zon ;;uror~  MySQL Serverless v2. Use ;;m~zon Simple Queue Service (;;m~zon SQS) for ~synchronous mess~ging.

 Correct ;;nswer: ;;
 D (95%)                                   5%

 Question #347
 ;; solutions ~rchitect h~s l~unched multiple ;;m~zon  EC2 inst~nces in ~ pl~cement group within ~ single ;;v~il~bility Zone.  Bec~use of ~ddition~l lo~d on the system, the solutions ~rchitect ~ttempts to ~dd new inst~nces to the pl~cement group.  However, the solutions ~rchitect receives ~n insu cient c~p~city error. Wh~t should the solutions ~rchitect do to troubleshoot this issue?
  ;;. Use ~ spre~d pl~cement group. Set ~ minimum of eight inst~nces for e~ch ;;v~il~bility Zone.
  B. Stop ~nd st~rt ~ll the inst~nces in the pl~cement group. Try the l~unch ~g~in.
  C. Cre~te ~ new pl~cement group.  Merge the new pl~cement group with the origin~l pl~cement group.
  D.  L~unch the ~ddition~l inst~nces ~s  Dedic~ted  Hosts in the pl~cement groups.

 Correct ;;nswer: C
 B (85%)                                  D (15%)

 Question #348
 ;; comp~ny h~s used infr~structure ~s code (I~C) to provision ~ set of two ;;m~zon  EC2 inst~nces. The inst~nces h~ve rem~ined the s~me for sever~l ye~rs. The comp~ny's business h~s grown r~pidly in the p~st few months.  In response, the comp~ny’s oper~tions te~m h~s implemented ~n ;;uto Sc~ling group to m~n~ge the sudden incre~ses in tr~ c. Comp~ny policy requires ~ monthly inst~ll~tion of security upd~tes on ~ll oper~ting systems th~t ~re running. The most recent security upd~te required ~ reboot. ;;s ~ result, the ;;uto Sc~ling group termin~ted the inst~nces ~nd repl~ced them with new, unp~tched inst~nces. Which combin~tion of steps should ~ solutions ~rchitect recommend to ~void ~ recurrence of this issue? (Choose two.)
  ;;.  Modify the ;;uto Sc~ling group by setting the Upd~te policy to t~rget the oldest l~unch con gur~tion for repl~cement.
  B. Cre~te ~ new ;;uto Sc~ling group before the next p~tch m~inten~nce.  During the m~inten~nce window, p~tch both groups ~nd reboot the inst~nces.
  C. Cre~te ~n  El~stic  Lo~d  B~l~ncer in front of the ;;uto Sc~ling group. Con gure monitoring to ensure th~t t~rget group he~lth checks return he~lthy ~fter the ;;uto Sc~ling group repl~ces the termin~ted inst~nces.
  D. Cre~te ~utom~tion scripts to p~tch ~n ;;MI, upd~te the l~unch con gur~tion, ~nd invoke ~n ;;uto Sc~ling inst~nce refresh.
  E. Cre~te ~n  El~stic  Lo~d  B~l~ncer in front of the ;;uto Sc~ling group. Con gure termin~tion protection on the inst~nces.

 Correct ;;nswer: ;;D
 CD (67%)                             ;;C (25%)         8%

 Question #349
 ;; te~m of d~t~ scientists is using ;;m~zon S~geM~ker inst~nces ~nd S~geM~ker ;;PIs to tr~in m~chine le~rning (ML) models. The S~geM~ker inst~nces ~re deployed in ~ VPC th~t does not h~ve ~ccess to or from the internet.  D~t~sets for  ML model tr~ining ~re stored in ~n ;;m~zon S3 bucket.  Interf~ce VPC endpoints provide ~ccess to ;;m~zon S3 ~nd the S~geM~ker ;;PIs. Occ~sion~lly, the d~t~ scientists require ~ccess to the  Python  P~ck~ge  Index (PyPI) repository to upd~te  Python p~ck~ges th~t they use ~s p~rt of their work ow. ;; solutions ~rchitect must provide ~ccess to the  PyPI repository while ensuring th~t the S~geM~ker inst~nces rem~in isol~ted from the internet. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;WS CodeCommit repository for e~ch p~ck~ge th~t the d~t~ scientists need to ~ccess. Con gure code synchroniz~tion between the  PyPI repository ~nd the CodeCommit repository. Cre~te ~ VPC endpoint for CodeCommit.
  B. Cre~te ~  N;;T g~tew~y in the VPC. Con gure VPC routes to ~llow ~ccess to the internet with ~ network ;;CL th~t ~llows ~ccess to only the PyPI repository endpoint.
  C. Cre~te ~  N;;T inst~nce in the VPCon gure VPC routes to ~llow ~ccess to the internet. Con gure S~geM~ker notebook inst~nce  rew~ll rules th~t ~llow ~ccess to only the  PyPI repository endpoint.
  D. Cre~te ~n ;;WS Code;;rtif~ct dom~in ~nd repository. ;;dd ~n extern~l connection for public:pypi to the Code;;rtif~ct repository. Con gure the Python client to use the Code;;rtif~ct repository. Cre~te ~ VPC endpoint for Code;;rtif~ct.

 Correct ;;nswer: C
 D (100%)

 Question #350
 ;; solutions ~rchitect works for ~ government ~gency th~t h~s strict dis~ster recovery requirements. ;;ll ;;m~zon  El~stic  Block Store (;;m~zon  EBS) sn~pshots ~re required to be s~ved in ~t le~st two ~ddition~l ;;WS  Regions. The ~gency ~lso is required to m~int~in the lowest possible oper~tion~l overhe~d. Which solution meets these requirements?
  ;;. Con gure ~ policy in ;;m~zon  D~t~  Lifecycle  M~n~ger (;;m~zon  DLM) to run once d~ily to copy the  EBS sn~pshots to the ~ddition~l  Regions.
  B. Use ;;m~zon  EventBridge to schedule ~n ;;WS  L~mbd~ function to copy the  EBS sn~pshots to the ~ddition~l  Regions.
  C. Setup ;;WS  B~ckup to cre~te the  EBS sn~pshots. Con gure ;;m~zon S3 Cross-Region  Replic~tion to copy the  EBS sn~pshots to the ~ddition~l  Regions.
  D. Schedule ;;m~zon  EC2  Im~ge  Builder to run once d~ily to cre~te ~n ;;MI ~nd copy the ;;MI to the ~ddition~l  Regions.

 Correct ;;nswer: ;;
 ;; (86%)                                    14%

 Question #351
 ;; comp~ny h~s ~ project th~t is l~unching ;;m~zon  EC2 inst~nces th~t ~re l~rger th~n required. The project's ~ccount c~nnot be p~rt of the comp~ny's org~niz~tion in ;;WS Org~niz~tions due to policy restrictions to keep this ~ctivity outside of corpor~te  IT. The comp~ny w~nts to ~llow only the l~unch of t3.sm~ll  EC2 inst~nces by developers in the project's ~ccount. These  EC2 inst~nces must be restricted to the us-e~st-2  Region. Wh~t should ~ solutions ~rchitect do to meet these requirements?
  ;;. Cre~te ~ new developer ~ccount.  Move ~ll  EC2 inst~nces, users, ~nd ~ssets into us-e~st-2. ;;dd the ~ccount to the comp~ny's org~niz~tion in ;;WS Org~niz~tions.  Enforce ~ t~gging policy th~t denotes  Region ~ nity.
  B. Cre~te ~n SCP th~t denies the l~unch of ~ll  EC2 inst~nces except t3.sm~ll  EC2 inst~nces in us-e~st-2. ;;tt~ch the SCP to the project's ~ccount.
  C. Cre~te ~nd purch~se ~ t3.sm~ll  EC2  Reserved  Inst~nce for e~ch developer in us-e~st-2. ;;ssign e~ch developer ~ speci c  EC2 inst~nce with their n~me ~s the t~g.
  D. Cre~te ~n  I;;M policy th~n ~llows the l~unch of only t3.sm~ll  EC2 inst~nces in us-e~st-2. ;;tt~ch the policy to the roles ~nd groups th~t the developers use in the project's ~ccount.

 Correct ;;nswer: B
 D (88%)                                    13%

 Question #352
 ;; scienti c comp~ny needs to process text ~nd im~ge d~t~ from ~n ;;m~zon S3 bucket. The d~t~ is collected from sever~l r~d~r st~tions during ~ live, time-critic~l ph~se of ~ deep sp~ce mission. The r~d~r st~tions uplo~d the d~t~ to the source S3 bucket. The d~t~ is pre xed by r~d~r st~tion identi c~tion number. The comp~ny cre~ted ~ destin~tion S3 bucket in ~ second ~ccount.  D~t~ must be copied from the source S3 bucket to the destin~tion S3 bucket to meet ~ compli~nce objective. This replic~tion occurs through the use of ~n S3 replic~tion rule to cover ~ll objects in the source S3 bucket. One speci c r~d~r st~tion is identi ed ~s h~ving the most ~ccur~te d~t~.  D~t~ replic~tion ~t this r~d~r st~tion must be monitored for completion within 30 minutes ~fter the r~d~r st~tion uplo~ds the objects to the source S3 bucket. Wh~t should ~ solutions ~rchitect do to meet these requirements?
  ;;. Setup ~n ;;WS  D~t~Sync ~gent to replic~te the pre xed d~t~ from the source S3 bucket to the destin~tion S3 bucket. Select to use ~ll ~v~il~ble b~ndwidth on the t~sk, ~nd monitor the t~sk to ensure th~t itis in the TR;;NSFERRING st~tus. Cre~te ~n ;;m~zon  EventBridge rule to initi~te ~n ~lert if this st~tus ch~nges.
  B.  In the second ~ccount, cre~te ~nother S3 bucket to receive d~t~ from the r~d~r st~tion with the most ~ccur~te d~t~. Set up ~ new replic~tion rule for this new S3 bucket to sep~r~te the replic~tion from the other r~d~r st~tions.  Monitor the m~ximum replic~tion time to the destin~tion. Cre~te ~n ;;m~zon  EventBridge rule to initi~te ~n ~lert when the time exceeds the desired threshold.
  C.  En~ble ;;m~zon S3 Tr~nsfer ;;cceler~tion on the source S3 bucket, ~nd con gure the r~d~r st~tion with the most ~ccur~te d~t~ to use the new endpoint.  Monitor the S3 destin~tion bucket's Tot~lRequestL~tency metric. Cre~te ~n ;;m~zon  EventBridge rule to initi~te ~n ~lert if this st~tus ch~nges.
  D. Cre~te ~ new S3 replic~tion rule on the source S3 bucket th~t  lters for the keys th~t use the pre x of the r~d~r st~tion with the most ~ccur~te d~t~.  En~ble S3  Replic~tion Time Control (S3  RTC).  Monitor the m~ximum replic~tion time to the destin~tion. Cre~te ~n ;;m~zon EventBridge rule to initi~te ~n ~lert when the time exceeds the desired threshold.

 Correct ;;nswer: C
 D (100%)

 Question #353
 ;; comp~ny w~nts to migr~te its on-premises d~t~ center to the ;;WS Cloud. This includes thous~nds of virtu~lized  Linux ~nd  Microsoft Windows servers, S;;N stor~ge, J~v~ ~nd  PHP ~pplic~tions with  MySQL, ~nd Or~cle d~t~b~ses. There ~re m~ny dependent services hosted either in the s~me d~t~ center or extern~lly. The technic~l document~tion is incomplete ~nd outd~ted. ;; solutions ~rchitect needs to underst~nd the current environment ~nd estim~te the cloud resource costs ~fter the migr~tion. Which tools or services should the solutions ~rchitect use to pl~n the cloud migr~tion? (Choose three.)
  ;;. ;;WS ;;pplic~tion  Discovery Service
  B. ;;WS SMS
  C. ;;WS X-R~y
  D. ;;WS Cloud ;;doption  Re~diness Tool (C;;RT)
  E. ;;m~zon  Inspector
  F. ;;WS  Migr~tion  Hub

 Correct ;;nswer: DEF
 ;;DF (72%)                            11%        Other

 Question #354
 ;; solutions ~rchitect is reviewing ~n ~pplic~tion's resilience before l~unch. The ~pplic~tion runs on ~n ;;m~zon  EC2 inst~nce th~t is deployed in ~ priv~te subnet of ~ VPC. The  EC2 inst~nce is provisioned by ~n ;;uto Sc~ling group th~t h~s ~ minimum c~p~city of  1 ~nd ~ m~ximum c~p~city of 1. The ~pplic~tion stores d~t~ on ~n ;;m~zon  RDS for  MySQL  DB inst~nce. The VPC h~s subnets con gured in three ;;v~il~bility Zones ~nd is con gured with ~ single  N;;T g~tew~y. The solutions ~rchitect needs to recommend ~ solution to ensure th~t the ~pplic~tion will oper~te ~cross multiple ;;v~il~bility Zones. Which solution will meet this requirement?
  ;;.  Deploy ~n ~ddition~l  N;;T g~tew~y in the other ;;v~il~bility Zones. Upd~te the route t~bles with ~ppropri~te routes.  Modify the  RDS for MySQL  DB inst~nce to ~  Multi-;;Z con gur~tion. Con gure the ;;uto Sc~ling group to l~unch the inst~nces ~cross ;;v~il~bility Zones. Set the minimum c~p~city ~nd m~ximum c~p~city of the ;;uto Sc~ling group to 3.
  B.  Repl~ce the  N;;T g~tew~y with ~ virtu~l priv~te g~tew~y.  Repl~ce the  RDS for  MySQL  DB inst~nce with ~n ;;m~zon ;;uror~  MySQL  DB cluster. Con gure the ;;uto Sc~ling group to l~unch inst~nces ~cross ~ll subnets in the VPC. Set the minimum c~p~city ~nd m~ximum c~p~city of the ;;uto Sc~ling group to 3.
  C.  Repl~ce the  N;;T g~tew~y with ~  N;;T inst~nce.  Migr~te the  RDS for  MySQL  DB inst~nce to ~n  RDS for  PostgreSQL  DB inst~nce.  L~unch ~ new  EC2 inst~nce in the other ;;v~il~bility Zones.
  D.  Deploy ~n ~ddition~l  N;;T g~tew~y in the other ;;v~il~bility Zones. Upd~te the route t~bles with ~ppropri~te routes.  Modify the  RDS for MySQL  DB inst~nce to turn on ~utom~tic b~ckups ~nd ret~in the b~ckups for 7 d~ys. Con gure the ;;uto Sc~ling group to l~unch inst~nces ~cross ~ll subnets in the VPC.  Keep the minimum c~p~city ~nd the m~ximum c~p~city of the ;;uto Sc~ling group ~t  1.

 Correct ;;nswer: C
 ;; (100%)

 Question #355
 ;; comp~ny is pl~nning to migr~te its on-premises tr~ns~ction-processing ~pplic~tion to ;;WS. The ~pplic~tion runs inside  Docker cont~iners th~t ~re hosted on VMs in the comp~ny's d~t~ center. The  Docker cont~iners h~ve sh~red stor~ge where the ~pplic~tion records tr~ns~ction d~t~. The tr~ns~ctions ~re time sensitive. The volume of tr~ns~ctions inside the ~pplic~tion is unpredict~ble. The comp~ny must implement ~ low- l~tency stor~ge solution th~t will ~utom~tic~lly sc~le throughput to meet incre~sed dem~nd. The comp~ny c~nnot develop the ~pplic~tion further ~nd c~nnot continue to ~dminister the  Docker hosting environment. How should the comp~ny migr~te the ~pplic~tion to ;;WS to meet these requirements?
  ;;.  Migr~te the cont~iners th~t run the ~pplic~tion to ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS). Use ;;m~zon S3 to store the tr~ns~ction d~t~ th~t the cont~iners sh~re.
  B.  Migr~te the cont~iners th~t run the ~pplic~tion to ;;WS  F~rg~te for ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS). Cre~te ~n ;;m~zon El~stic  File System (;;m~zon  EFS)  le system. Cre~te ~  F~rg~te t~sk de nition. ;;dd ~ volume to the t~sk de nition to point to the  EFS  le system.
  C.  Migr~te the cont~iners th~t run the ~pplic~tion to ;;WS  F~rg~te for ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS). Cre~te ~n ;;m~zon El~stic  Block Store (;;m~zon  EBS) volume. Cre~te ~  F~rg~te t~sk de nition. ;;tt~ch the  EBS volume to e~ch running t~sk.
  D.  L~unch ;;m~zon  EC2 inst~nces.  Inst~ll  Docker on the  EC2 inst~nces.  Migr~te the cont~iners to the  EC2 inst~nces. Cre~te ~n ;;m~zon  El~stic File System (;;m~zon  EFS)  le system. ;;dd ~ mount point to the  EC2 inst~nces for the  EFS  le system.

 Correct ;;nswer: ;;
 B (100%)

 Question #356
 ;; comp~ny is pl~nning to migr~te to the ;;WS Cloud. The comp~ny hosts m~ny ~pplic~tions on Windows servers ~nd  Linux servers. Some of the servers ~re physic~l, ~nd some of the servers ~re virtu~l. The comp~ny uses sever~l types of d~t~b~ses in its on-premises environment. The comp~ny does not h~ve ~n ~ccur~te inventory of its on-premises servers ~nd ~pplic~tions. The comp~ny w~nts to rightsize its resources during migr~tion. ;; solutions ~rchitect needs to obt~in inform~tion ~bout the network connections ~nd the ~pplic~tion rel~tionships. The solutions ~rchitect must ~ssess the comp~ny’s current environment ~nd develop ~ migr~tion pl~n. Which solution will provide the solutions ~rchitect with the required inform~tion to develop the migr~tion pl~n?
  ;;. Use  Migr~tion  Ev~lu~tor to request ~n ev~lu~tion of the environment from ;;WS. Use the ;;WS ;;pplic~tion  Discovery Service ;;gentless Collector to import the det~ils into ~  Migr~tion  Ev~lu~tor Quick  Insights report.
  B. Use ;;WS  Migr~tion  Hub ~nd inst~ll the ;;WS ;;pplic~tion  Discovery ;;gent on the servers.  Deploy the  Migr~tion  Hub Str~tegy Recommend~tions ~pplic~tion d~t~ collector. Gener~te ~ report by using  Migr~tion  Hub Str~tegy  Recommend~tions.
  C. Use ;;WS  Migr~tion  Hub ~nd run the ;;WS ;;pplic~tion  Discovery Service ;;gentless Collector on the servers. Group the servers ~nd d~t~b~ses by using ;;WS ;;pplic~tion  Migr~tion Service. Gener~te ~ report by using  Migr~tion  Hub Str~tegy  Recommend~tions.
  D. Use the ;;WS  Migr~tion  Hub import tool to lo~d the det~ils of the comp~ny’s on-premises environment. Gener~te ~ report by using  Migr~tion Hub Str~tegy  Recommend~tions.

 Correct ;;nswer: D
 B (100%)

 Question #357
 ;;  n~nci~l services comp~ny sells its softw~re-~s-~-service (S~~S) pl~tform for ~pplic~tion compli~nce to l~rge glob~l b~nks. The S~~S pl~tform runs on ;;WS ~nd uses multiple ;;WS ~ccounts th~t ~re m~n~ged in ~n org~niz~tion in ;;WS Org~niz~tions. The S~~S pl~tform uses m~ny ;;WS resources glob~lly. For regul~tory compli~nce, ~ll ;;PI c~lls to ;;WS resources must be ~udited, tr~cked for ch~nges, ~nd stored in ~ dur~ble ~nd secure d~t~ store. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ new ;;WS CloudTr~il tr~il. Use ~n existing ;;m~zon S3 bucket in the org~niz~tion's m~n~gement ~ccount to store the logs.  Deploy the tr~il to ~ll ;;WS  Regions.  En~ble  MF;; delete ~nd encryption on the S3 bucket.
  B. Cre~te ~ new ;;WS CloudTr~il tr~il in e~ch member ~ccount of the org~niz~tion. Cre~te new ;;m~zon S3 buckets to store the logs.  Deploy the tr~il to ~ll ;;WS  Regions.  En~ble  MF;; delete ~nd encryption on the S3 buckets.
  C. Cre~te ~ new ;;WS CloudTr~il tr~il in the org~niz~tion's m~n~gement ~ccount. Cre~te ~ new ;;m~zon S3 bucket with versioning turned on to store the logs.  Deploy the tr~il for ~ll ~ccounts in the org~niz~tion.  En~ble  MF;; delete ~nd encryption on the S3 bucket.
  D. Cre~te ~ new ;;WS CloudTr~il tr~il in the org~niz~tion's m~n~gement ~ccount. Cre~te ~ new ;;m~zon S3 bucket to store the logs. Con gure ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to send log- le delivery noti c~tions to ~n extern~l m~n~gement system th~t will tr~ck the logs.  En~ble  MF;; delete ~nd encryption on the S3 bucket.

 Correct ;;nswer: C
 C (90%)                                    10%

 Question #358
 ;; comp~ny is deploying ~ distributed in-memory d~t~b~se on ~  eet of ;;m~zon  EC2 inst~nces. The  eet consists of ~ prim~ry node ~nd eight worker nodes. The prim~ry node is responsible for monitoring cluster he~lth, ~ccepting user requests, distributing user requests to worker nodes, ~nd sending ~n ~ggreg~te response b~ck to ~ client. Worker nodes communic~te with e~ch other to replic~te d~t~ p~rtitions. The comp~ny requires the lowest possible networking l~tency to ~chieve m~ximum perform~nce. Which solution will meet these requirements?
  ;;.  L~unch memory optimized  EC2 inst~nces in ~ p~rtition pl~cement group.
  B.  L~unch compute optimized  EC2 inst~nces in ~ p~rtition pl~cement group.
  C.  L~unch memory optimized  EC2 inst~nces in ~ cluster pl~cement group.
  D.  L~unch compute optimized  EC2 inst~nces in ~ spre~d pl~cement group.

 Correct ;;nswer: C
 C (100%)

 Question #359
 ;; comp~ny m~int~ins inform~tion on premises in ~pproxim~tely  1 million.csv  les th~t ~re hosted on ~ VM. The d~t~ initi~lly is  10 TB in size ~nd grows ~t ~ r~te of  1 TB e~ch week. The comp~ny needs to ~utom~te b~ckups of the d~t~ to the ;;WS Cloud. B~ckups of the d~t~ must occur d~ily. The comp~ny needs ~ solution th~t ~pplies custom  lters to b~ck up only ~ subset of the d~t~ th~t is loc~ted in design~ted source directories. The comp~ny h~s set up ~n ;;WS  Direct Connect connection. Which solution will meet the b~ckup requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Use the ;;m~zon S3 CopyObject ;;PI oper~tion with multip~rt uplo~d to copy the existing d~t~ to ;;m~zon S3. Use the CopyObject ;;PI oper~tion to replic~te new d~t~ to ;;m~zon S3 d~ily.
  B. Cre~te ~ b~ckup pl~n in ;;WS  B~ckup to b~ck up the d~t~ to ;;m~zon S3. Schedule the b~ckup pl~n to run d~ily.
  C.  Inst~ll the ;;WS  D~t~Sync ~gent ~s ~ VM th~t runs on the on-premises hypervisor. Con gure ~  D~t~Sync t~sk to replic~te the d~t~ to ;;m~zon S3 d~ily.
  D. Use ~n ;;WS Snowb~ll  Edge device for the initi~l b~ckup. Use ;;WS  D~t~Sync for increment~l b~ckups to ;;m~zon S3 d~ily.

 Correct ;;nswer: D
 C (82%)                                  B (18%)

 Question #360
 ;;  n~nci~l services comp~ny h~s ~n ~sset m~n~gement product th~t thous~nds of customers use ~round the world. The customers provide feedb~ck ~bout the product through surveys. The comp~ny is building ~ new ~n~lytic~l solution th~t runs on ;;m~zon  EMR to ~n~lyze the d~t~ from these surveys. The following user person~s need to ~ccess the ~n~lytic~l solution to perform different ~ctions: • ;;dministr~tor:  Provisions the  EMR cluster for the ~n~lytics te~m b~sed on the te~m’s requirements •  D~t~ engineer:  Runs  ETL scripts to process, tr~nsform, ~nd enrich the d~t~sets •  D~t~ ~n~lyst:  Runs SQL ~nd  Hive queries on the d~t~ ;; solutions ~rchitect must ensure th~t ~ll the user person~s h~ve le~st privilege ~ccess to only the resources th~t they need. The user person~s must be ~ble to l~unch only ~pplic~tions th~t ~re ~pproved ~nd ~uthorized. The solution ~lso must ensure t~gging for ~ll resources th~t the user person~s cre~te. Which solution will meet these requirements?
  ;;. Cre~te  I;;M roles for e~ch user person~. ;;tt~ch identity-b~sed policies to de ne which ~ctions the user who ~ssumes the role c~n perform. Cre~te ~n ;;WS Con g rule to check for noncompli~nt resources. Con gure the rule to notify the ~dministr~tor to remedi~te the noncompli~nt resources.
  B. Setup  Kerberos-b~sed ~uthentic~tion for  EMR clusters upon l~unch. Specify ~  Kerberos security con gur~tion ~long with cluster-speci c Kerberos options.
  C. Use ;;WS Service C~t~log to control the ;;m~zon  EMR versions ~v~il~ble for deployment, the cluster con gur~tion, ~nd the permissions for e~ch user person~.
  D.  L~unch the  EMR cluster by using ;;WS CloudForm~tion, ;;tt~ch resource-b~sed policies to the  EMR cluster during cluster cre~tion. Cre~te ~n ;;WS. Con g rule to check for noncompli~nt clusters ~nd noncompli~nt ;;m~zon S3 buckets. Con gure the rule to notify the ~dministr~tor to remedi~te the noncompli~nt resources.

 Correct ;;nswer: ;;
 C (79%)                                 ;; (21%)

 Question #361
 ;; softw~re ~s ~ service (S~~S) comp~ny uses ;;WS to host ~ service th~t is powered by ;;WS  Priv~teLink. The service consists of propriet~ry softw~re th~t runs on three ;;m~zon  EC2 inst~nces behind ~  Network  Lo~d  B~l~ncer (NLB). The inst~nces ~re in priv~te subnets in multiple ;;v~il~bility Zones in the eu-west-2  Region. ;;ll the comp~ny's customers ~re in eu-west-2. However, the comp~ny now ~cquires ~ new customer in the us-e~st-1  Region. The comp~ny cre~tes ~ new VPC ~nd new subnets in us-e~st-1. The comp~ny est~blishes inter-Region VPC peering between the VPCs in the two  Regions. The comp~ny w~nts to give the new customer ~ccess to the S~~S service, but the comp~ny does not w~nt to immedi~tely deploy new  EC2 resources in us-e~st-1. Which solution will meet these requirements?
  ;;. Con gure ~  Priv~teLink endpoint service in us-e~st-1 to use the existing  NLB th~t is in eu-west-2. Gr~nt speci c ;;WS ~ccounts ~ccess to connect to the S~~S service.
  B. Cre~te ~n  NLB in us-e~st-1. Cre~te ~n  IP t~rget group th~t uses the  IP ~ddresses of the comp~ny's inst~nces in eu-west-2 th~t host the S~~S service. Con gure ~  Priv~teLink endpoint service th~t uses the  NLB th~t is in us-e~st-1. Gr~nt speci c ;;WS ~ccounts ~ccess to connect to the S~~S service.
  C. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) in front of the  EC2 inst~nces in eu-west-2. Cre~te ~n  NLB in us-e~st-1. ;;ssoci~te the  NLB th~t is in us-e~st-1 with ~n ;;LB t~rget group th~t uses the ;;LB th~t is in eu-west-2. Con gure ~  Priv~teLink endpoint service th~t uses the  NLB th~t is in us-e~st-1. Gr~nt speci c ;;WS ~ccounts ~ccess to connect to the S~~S service.
  D. Use ;;WS  Resource ;;ccess  M~n~ger (;;WS  R;;M) to sh~re the  EC2 inst~nces th~t ~re in eu-west-2.  In us-e~st-1, cre~te ~n  NLB ~nd ~n inst~nce t~rget group th~t includes the sh~red  EC2 inst~nces from eu-west-2. Con gure ~  Priv~teLink endpoint service th~t uses the  NLB th~t is in us-e~st-1. Gr~nt speci c ;;WS ~ccounts ~ccess to connect to the S~~S service.

 Correct ;;nswer: D
 B (56%)                                  ;; (44%)

 Question #362
 ;; comp~ny needs to monitor ~ growing number of ;;m~zon S3 buckets ~cross two ;;WS  Regions. The comp~ny ~lso needs to tr~ck the percent~ge of objects th~t ~re encrypted in ;;m~zon S3. The comp~ny needs ~ d~shbo~rd to displ~y this inform~tion for intern~l compli~nce te~ms. Which solution will meet these requirements with the  LE;;ST oper~tion~l overhe~d?
  ;;. Cre~te ~ new 3 Stor~ge  Lens d~shbo~rd in e~ch  Region to tr~ck bucket ~nd encryption metrics. ;;ggreg~te d~t~ from both  Region d~shbo~rds into ~ single d~shbo~rd in ;;m~zon QuickSight for the compli~nce te~ms.
  B.  Deploy ~n ;;WS  L~mbd~ function in e~ch  Region to list the number of buckets ~nd the encryption st~tus of objects. Store this d~t~ in ;;m~zon S3. Use ;;m~zon ;;then~ queries to displ~y the d~t~ on ~ custom d~shbo~rd in ;;m~zon QuickSight for the compli~nce te~ms.
  C. Use the S3 Stor~ge  Lens def~ult d~shbo~rd to tr~ck bucket ~nd encryption metrics. Give the compli~nce te~ms ~ccess to the d~shbo~rd directly in the S3 console.
  D. Cre~te ~n ;;m~zon  EventBridge rule to detect ;;WS CloudTr~il events for S3 object cre~tion. Con gure the rule to invoke ~n ;;WS  L~mbd~ function to record encryption metrics in ;;m~zon  Dyn~moDB. Use ;;m~zon QuickSight to displ~y the metrics in ~ d~shbo~rd for the compli~nce te~ms.

 Correct ;;nswer: B
 C (80%)                               13%      7%

 Question #363
 ;; comp~ny’s CISO h~s ~sked ~ solutions ~rchitect to re-engineer the comp~ny's current CI/CD pr~ctices to m~ke sure p~tch deployments to its ~pplic~tion c~n h~ppen ~s quickly ~s possible with minim~l downtime if vulner~bilities ~re discovered. The comp~ny must ~lso be ~ble to quickly roll b~ck ~ ch~nge in c~se of errors. The web ~pplic~tion is deployed in ~  eet of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer. The comp~ny is currently using GitHub to host the ~pplic~tion source code, ~nd h~s con gured ~n ;;WS CodeBuild project to build the ~pplic~tion. The comp~ny ~lso intends to use ;;WS CodePipeline to trigger builds from GitHub commits using the existing CodeBuild project. Wh~t CI/CD con gur~tion meets ~ll of the requirements?
  ;;. Con gure CodePipeline with ~ deploy st~ge using ;;WS CodeDeploy con gured for in-pl~ce deployment.  Monitor the newly deployed code, ~nd, if there ~re ~ny issues, push ~nother code upd~te
  B. Con gure CodePipeline with ~ deploy st~ge using ;;WS CodeDeploy con gured for blue/green deployments.  Monitor the newly deployed code, ~nd, if there ~re ~ny issues, trigger ~ m~nu~l rollb~ck using CodeDeploy.
  C. Con gure CodePipeline with ~ deploy st~ge using ;;WS CloudForm~tion to cre~te ~ pipeline for test ~nd production st~cks.  Monitor the newly deployed code, ~nd, if there ~re ~ny issues, push ~nother code upd~te.
  D. Con gure the CodePipeline with ~ deploy st~ge using ;;WS OpsWorks ~nd in-pl~ce deployments.  Monitor the newly deployed code, ~nd, if there ~re ~ny issues, push ~nother code upd~te.

 Correct ;;nswer: C
 B (100%)

 Question #364
 ;; comp~ny is m~n~ging m~ny ;;WS ~ccounts by using ~n org~niz~tion in ;;WS Org~niz~tions.  Different business units in the comp~ny run ~pplic~tions on ;;m~zon  EC2 inst~nces. ;;ll the  EC2 inst~nces must h~ve ~  BusinessUnit t~g so th~t the comp~ny c~n tr~ck the cost for e~ch business unit. ;; recent ~udit reve~led th~t some inst~nces were missing this t~g. The comp~ny m~nu~lly ~dded the missing t~g to the inst~nces. Wh~t should ~ solutions ~rchitect do to enforce the t~gging requirement in the future?
  ;;.  En~ble t~g policies in the org~niz~tion. Cre~te ~ t~g policy for the  BusinessUnit t~g.  Ensure th~t compli~nce with t~g key c~pit~liz~tion is turned off.  Implement the t~g policy for the ec2:inst~nce resource type. ;;tt~ch the t~g policy to the root of the org~niz~tion.
  B.  En~ble t~g policies in the org~niz~tion. Cre~te ~ t~g policy for the  BusinessUnit t~g.  Ensure th~t compli~nce with t~g key c~pit~liz~tion is turned on.  Implement the t~g policy for the ec2:inst~nce resource type. ;;tt~ch the t~g policy to the org~niz~tion's m~n~gement ~ccount.
  C. Cre~te ~n SCP ~nd ~tt~ch the SCP to the root of the org~niz~tion.  Include the following st~tement in the SCP:
  D. Cre~te ~n SCP ~nd ~tt~ch the SCP to the org~niz~tion’s m~n~gement ~ccount.  Include the following st~tement in the SCP:

 Correct ;;nswer: B
 C (54%)                              B (35%)              8%

 Question #365
 ;; comp~ny is running ~ worklo~d th~t consists of thous~nds of ;;m~zon  EC2 inst~nces. The worklo~d is running in ~ VPC th~t cont~ins sever~l public subnets ~nd priv~te subnets. The public subnets h~ve ~ route for 0.0.0.0/0 to ~n existing internet g~tew~y. The priv~te subnets h~ve ~ route for 0.0.0.0/0 to ~n existing  N;;T g~tew~y. ;; solutions ~rchitect needs to migr~te the entire  eet of  EC2 inst~nces to use  IPv6. The  EC2 inst~nces th~t ~re in priv~te subnets must not be ~ccessible from the public internet. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Upd~te the existing VPC, ~nd ~ssoci~te ~ custom  IPv6 CIDR block with the VPC ~nd ~ll subnets. Upd~te ~ll the VPC route t~bles, ~nd ~dd ~ route for ::/0 to the internet g~tew~y.
  B. Upd~te the existing VPC, ~nd ~ssoci~te ~n ;;m~zon-provided  IPv6 CIDR block with the VPC ~nd ~ll subnets. Upd~te the VPC route t~bles for ~ll priv~te subnets, ~nd ~dd ~ route for ::/0 to the  N;;T g~tew~y.
  C. Upd~te the existing VPC, ~nd ~ssoci~te ~n ;;m~zon-provided  IPv6 CIDR block with the VPC ~nd ~ll subnets. Cre~te ~n egress-only internet g~tew~y. Upd~te the VPC route t~bles for ~ll priv~te subnets, ~nd ~dd ~ route for ::/0 to the egress-only internet g~tew~y.
  D. Upd~te the existing VPC, ~nd ~ssoci~te ~ custom  IPV6 CIDR block with the VPC ~nd ~ll subnets. Cre~te ~ new  N;;T g~tew~y, ~nd en~ble IPV6 support. Upd~te the VPC route t~bles for ~ll priv~te subnets, ~nd ~dd ~ route for ::/0 to the  IPv6-en~bled  N;;T g~tew~y.

 Correct ;;nswer: C
 C (88%)                                    12%

 Question #366
 ;; comp~ny is using ;;m~zon ;;PI G~tew~y to deploy ~ priv~te  REST ;;PI th~t will provide ~ccess to sensitive d~t~. The ;;PI must be ~ccessible only from ~n ~pplic~tion th~t is deployed in ~ VPC. The comp~ny deploys the ;;PI successfully.  However, the ;;PI is not ~ccessible from ~n ;;m~zon  EC2 inst~nce th~t is deployed in the VPC. Which solution will provide connectivity between the  EC2 inst~nce ~nd the ;;PI?
  ;;. Cre~te ~n interf~ce VPC endpoint for ;;PI G~tew~y. ;;tt~ch ~n endpoint policy th~t ~llows ~pig~tew~y:* ~ctions.  Dis~ble priv~te  DNS n~ming for the VPC endpoint. Con gure ~n ;;PI resource policy th~t ~llows ~ccess from the VPC. Use the VPC endpoint's  DNS n~me to ~ccess the ;;PI.
  B. Cre~te ~n interf~ce VPC endpoint for ;;PI G~tew~y. ;;tt~ch ~n endpoint policy th~t ~llows the execute-~pi:Invoke ~ction.  En~ble priv~te  DNS n~ming for the VPC endpoint. Con gure ~n ;;PI resource policy th~t ~llows ~ccess from the VPC endpoint. Use the ;;PI endpoint’s  DNS n~mes to ~ccess the ;;PI.
  C. Cre~te ~  Network  Lo~d  B~l~ncer (NLB) ~nd ~ VPC link. Con gure priv~te integr~tion between ;;PI G~tew~y ~nd the  NLB. Use the ;;PI endpoint’s  DNS n~mes to ~ccess the ;;PI.
  D. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) ~nd ~ VPC  Link. Con gure priv~te integr~tion between ;;PI G~tew~y ~nd the ;;LB. Use the ;;LB endpoint’s  DNS n~me to ~ccess the ;;PI.

 Correct ;;nswer: D
 B (100%)

 Question #367
 ;; l~rge p~yroll comp~ny recently merged with ~ sm~ll st~ ng comp~ny. The uni ed comp~ny now h~s multiple business units, e~ch with its own existing ;;WS ~ccount. ;; solutions ~rchitect must ensure th~t the comp~ny c~n centr~lly m~n~ge the billing ~nd ~ccess policies for ~ll the ;;WS ~ccounts. The solutions ~rchitect con gures ;;WS Org~niz~tions by sending ~n invit~tion to ~ll member ~ccounts of the comp~ny from ~ centr~lized m~n~gement ~ccount. Wh~t should the solutions ~rchitect do next to meet these requirements?
  ;;. Cre~te the Org~niz~tion;;ccount;;ccess  I;;M group in e~ch member ~ccount.  Include the necess~ry  I;;M roles for e~ch ~dministr~tor.
  B. Cre~te the Org~niz~tion;;ccount;;ccessPolicy  I;;M policy in e~ch member ~ccount. Connect the member ~ccounts to the m~n~gement ~ccount by using cross-~ccount ~ccess.
  C. Cre~te the Org~niz~tion;;ccount;;ccessRole  I;;M role in e~ch member ~ccount. Gr~nt permission to the m~n~gement ~ccount to ~ssume the  I;;M role.
  D. Cre~te the Org~niz~tion;;ccount;;ccessRole  I;;M role in the m~n~gement ~ccount. ;;tt~ch the ;;dministr~tor;;ccess ;;WS m~n~ged policy to the  I;;M role. ;;ssign the  I;;M role to the ~dministr~tors in e~ch member ~ccount.

 Correct ;;nswer: B
 C (89%)                                   11%

 Question #368
 ;; comp~ny h~s ~pplic~tion services th~t h~ve been cont~inerized ~nd deployed on multiple ;;m~zon  EC2 inst~nces with public  IPs. ;;n ;;p~che K~fk~ cluster h~s been deployed to the  EC2 inst~nces. ;;  PostgreSQL d~t~b~se h~s been migr~ted to ;;m~zon  RDS for  PostgreSQL. The comp~ny expects ~ signi c~nt incre~se of orders on its pl~tform when ~ new version of its  ~gship product is rele~sed. Wh~t ch~nges to the current ~rchitecture will reduce oper~tion~l overhe~d ~nd support the product rele~se?
  ;;. Cre~te ~n  EC2 ;;uto Sc~ling group behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Cre~te ~ddition~l re~d replic~s for the  DB inst~nce. Cre~te ;;m~zon Kinesis d~t~ stre~ms ~nd con gure the ~pplic~tion services to use the d~t~ stre~ms. Store ~nd serve st~tic content directly from ;;m~zon S3.
  B. Cre~te ~n  EC2 ;;uto Sc~ling group behind ~n ;;pplic~tion  Lo~d  B~l~ncer.  Deploy the  DB inst~nce in  Multi-;;Z mode ~nd en~ble stor~ge ~uto sc~ling. Cre~te ;;m~zon  Kinesis d~t~ stre~ms ~nd con gure the ~pplic~tion services to use the d~t~ stre~ms. Store ~nd serve st~tic content directly from ;;m~zon S3.
  C.  Deploy the ~pplic~tion on ~  Kubernetes cluster cre~ted on the  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer.  Deploy the  DB inst~nce in  Multi-;;Z mode ~nd en~ble stor~ge ~uto sc~ling. Cre~te ~n ;;m~zon  M~n~ged Stre~ming for ;;p~che  K~fk~ cluster ~nd con gure the ~pplic~tion services to use the cluster. Store st~tic content in ;;m~zon S3 behind ~n ;;m~zon CloudFront distribution.
  D.  Deploy the ~pplic~tion on ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) with ;;WS  F~rg~te ~nd en~ble ~uto sc~ling behind ~n ;;pplic~tion  Lo~d  B~l~ncer. Cre~te ~ddition~l re~d replic~s for the  DB inst~nce. Cre~te ~n ;;m~zon  M~n~ged Stre~ming for ;;p~che  K~fk~ cluster ~nd con gure the ~pplic~tion services to use the cluster. Store st~tic content in ;;m~zon S3 behind ~n ;;m~zon CloudFront distribution.

 Correct ;;nswer: ;;
 D (100%)

 Question #369
 ;; comp~ny hosts ~ VPN in ~n on-premises d~t~ center.  Employees currently connect to the VPN to ~ccess  les in their Windows home directories. Recently, there h~s been ~ l~rge growth in the number of employees who work remotely. ;;s ~ result, b~ndwidth us~ge for connections into the d~t~ center h~s begun to re~ch  100% during business hours. The comp~ny must design ~ solution on ;;WS th~t will support the growth of the comp~ny's remote workforce, reduce the b~ndwidth us~ge for connections into the d~t~ center, ~nd reduce oper~tion~l overhe~d. Which combin~tion of steps will meet these requirements with the  LE;;ST oper~tion~l overhe~d? (Choose two.)
  ;;. Cre~te ~n ;;WS Stor~ge G~tew~y Volume G~tew~y.  Mount ~ volume from the Volume G~tew~y to the on-premises  le server.
  B.  Migr~te the home directories to ;;m~zon  FSx for Windows  File Server.
  C.  Migr~te the home directories to ;;m~zon  FSx for  Lustre.
  D.  Migr~te remote users to ;;WS Client VPN.
  E. Cre~te ~n ;;WS  Direct Connect connection from the on-premises d~t~ center to ;;WS.

 Correct ;;nswer: BE
 BD (100%)

 Question #370
 ;; comp~ny h~s multiple ;;WS ~ccounts. The comp~ny recently h~d ~ security ~udit th~t reve~led m~ny unencrypted ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volumes ~tt~ched to ;;m~zon  EC2 inst~nces. ;; solutions ~rchitect must encrypt the unencrypted volumes ~nd ensure th~t unencrypted volumes will be detected ~utom~tic~lly in the future. ;;ddition~lly, the comp~ny w~nts ~ solution th~t c~n centr~lly m~n~ge multiple ;;WS ~ccounts with ~ focus on compli~nce ~nd security. Which combin~tion of steps should the solutions ~rchitect t~ke to meet these requirements? (Choose two.)
  ;;. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Set up ;;WS Control Tower, ~nd turn on the strongly recommended controls (gu~rdr~ils). Join ~ll ~ccounts to the org~niz~tion. C~tegorize the ;;WS ~ccounts into OUs.
  B. Use the ;;WS CLI to list ~ll the unencrypted volumes in ~ll the ;;WS ~ccounts.  Run ~ script to encrypt ~ll the unencrypted volumes in pl~ce.
  C. Cre~te ~ sn~pshot of e~ch unencrypted volume. Cre~te ~ new encrypted volume from the unencrypted sn~pshot.  Det~ch the existing volume, ~nd repl~ce it with the encrypted volume.
  D. Cre~te ~n org~niz~tion in ;;WS Org~niz~tions. Set up ;;WS Control Tower, ~nd turn on the m~nd~tory controls (gu~rdr~ils). Join ~ll ~ccounts to the org~niz~tion. C~tegorize the ;;WS ~ccounts into OUs.
  E. Turn on ;;WS CloudTr~il. Con gure ~n ;;m~zon  EventBridge rule to detect ~nd ~utom~tic~lly encrypt unencrypted volumes.

 Correct ;;nswer: CD
 ;;C (75%)                                 ;;E (25%)

 Question #371
 ;; comp~ny hosts ~n intr~net web ~pplic~tion on ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Currently, users ~uthentic~te to the ~pplic~tion ~g~inst ~n intern~l user d~t~b~se. The comp~ny needs to ~uthentic~te users to the ~pplic~tion by using ~n existing ;;WS  Directory Service for  Microsoft ;;ctive  Directory directory. ;;ll users with ~ccounts in the directory must h~ve ~ccess to the ~pplic~tion. Which solution will meet these requirements?
  ;;. Cre~te ~ new ~pp client in the directory. Cre~te ~ listener rule for the ;;LB. Specify the ~uthentic~te-oidc ~ction for the listener rule. Con gure the listener rule with the ~ppropri~te issuer, client  ID ~nd secret, ~nd endpoint det~ils for the ;;ctive  Directory service. Con gure the new ~pp client with the c~llb~ck URL th~t the ;;LB provides.
  B. Con gure ~n ;;m~zon Cognito user pool. Con gure the user pool with ~ feder~ted identity provider (ldP) th~t h~s met~d~t~ from the directory. Cre~te ~n ~pp client. ;;ssoci~te the ~pp client with the user pool. Cre~te ~ listener rule for the ;;LSpecify the ~uthentic~te-cognito ~ction for the listener rule. Con gure the listener rule to use the user pool ~nd ~pp client.
  C. ;;dd the directory ~s ~ new  I;;M identity provider (ldP). Cre~te ~ new  I;;M role th~t h~s ~n entity type of S;;ML 2.0 feder~tion. Con gure ~ role policy th~t ~llows ~ccess to the ;;LB. Con gure the new role ~s the def~ult ~uthentic~ted user role for the ldP. Cre~te ~ listener rule for the ;;LB. Specify the ~uthentic~te-oidc ~ction for the listener rule.
  D.  En~ble ;;WS  I;;M  Identity Center (;;WS Single Sign-On). Con gure the directory ~s ~n extern~l identity provider (ldP) th~t uses S;;ML. Use the ~utom~tic provisioning method. Cre~te ~ new  I;;M role th~t h~s ~n entity type of S;;ML 2.0 feder~tion. Con gure ~ role policy th~t ~llows ~ccess to the ;;LB. ;;tt~ch the new role to ~ll groups. Cre~te ~ listener rule for the ;;LB. Specify the ~uthentic~te-cognito ~ction for the listener rule.

 Correct ;;nswer: C
 B (42%)                         D (37%)                 ;; (21%)

 Question #372
 ;; comp~ny h~s ~ website th~t serves m~ny visitors. The comp~ny deploys ~ b~ckend service for the website in ~ prim~ry ;;WS  Region ~nd ~ dis~ster recovery (DR)  Region. ;; single ;;m~zon CloudFront distribution is deployed for the website. The comp~ny cre~tes ~n ;;m~zon  Route 53 record set with he~lth checks ~nd ~ f~ilover routing policy for the prim~ry  Region’s b~ckend service. The comp~ny con gures the  Route 53 record set ~s ~n origin for the CloudFront distribution. The comp~ny con gures ~nother record set th~t points to the b~ckend service's endpoint in the  DR  Region ~s ~ second~ry f~ilover record type. The TTL for both record sets is 60 seconds. Currently, f~ilover t~kes more th~n  1 minute. ;; solutions ~rchitect must design ~ solution th~t will provide the f~stest f~ilover time. Which solution will ~chieve this go~l?
  ;;.  Deploy ~n ~ddition~l CloudFront distribution. Cre~te ~ new  Route 53 f~ilover record set with he~lth checks for both CloudFront distributions.
  B. Set the TTL to 4 second for the existing  Route 53 record sets th~t ~re used for the b~ckend service in e~ch  Region.
  C. Cre~te new record sets for the b~ckend services by using ~ l~tency routing policy. Use the record sets ~s ~n origin in the CloudFront distribution.
  D. Cre~te ~ CloudFront origin group th~t includes two origins, one for e~ch b~ckend service  Region. Con gure origin f~ilover ~s ~ c~che beh~vior for the CloudFront distribution.

 Correct ;;nswer: B
 D (100%)

 Question #373
 ;; comp~ny is using multiple ;;WS ~ccounts ~nd h~s multiple  DevOps te~ms running production ~nd non-production worklo~ds in these ~ccounts. The comp~ny would like to centr~lly-restrict ~ccess to some of the ;;WS services th~t the  DevOps te~ms do not use. The comp~ny decided to use ;;WS Org~niz~tions ~nd successfully invited ~ll ;;WS ~ccounts into the Org~niz~tion. They would like to ~llow ~ccess to services th~t ~re currently in-use ~nd deny ~ few speci c services. ;;lso they would like to ~dminister multiple ~ccounts together ~s ~ single unit. Wh~t combin~tion of steps should the solutions ~rchitect t~ke to s~tisfy these requirements? (Choose three.)
  ;;. Use ~  Deny list str~tegy.
  B.  Review the ;;ccess ;;dvisor in ;;WS  I;;M to determine services recently used
  C.  Review the ;;WS Trusted ;;dvisor report to determine services recently used.
  D.  Remove the def~ult  Full;;WS;;ccess SCP.
  E.  De ne org~niz~tion~l units (OUs) ~nd pl~ce the member ~ccounts in the OUs.
  F.  Remove the def~ult  Deny;;WS;;ccess SCP.

 Correct ;;nswer: CDF
 ;;BE (89%)                                   11%

 Question #374
 ;; live-events comp~ny is designing ~ sc~ling solution for its ticket ~pplic~tion on ;;WS. The ~pplic~tion h~s high pe~ks of utiliz~tion during s~le events.  E~ch s~le event is ~ one-time event th~t is scheduled. The ~pplic~tion runs on ;;m~zon  EC2 inst~nces th~t ~re in ~n ;;uto Sc~ling group. The ~pplic~tion uses  PostgreSQL for the d~t~b~se l~yer. The comp~ny needs ~ sc~ling solution to m~ximize ~v~il~bility during the s~le events. Which solution will meet these requirements?
  ;;. Use ~ predictive sc~ling policy for the  EC2 inst~nces.  Host the d~t~b~se on ~n ;;m~zon ;;uror~  PostgreSQL Serverless v2  Multi-;;Z  DB inst~nce with ~utom~tic~lly sc~ling re~d replic~s. Cre~te ~n ;;WS Step  Functions st~te m~chine to run p~r~llel ;;WS  L~mbd~ functions to pre- w~rm the d~t~b~se before ~ s~le event. Cre~te ~n ;;m~zon  EventBridge rule to invoke the st~te m~chine.
  B. Use ~ scheduled sc~ling policy for the  EC2 inst~nces.  Host the d~t~b~se on ~n ;;m~zon  RDS for  PostgreSQL  Mulli-;;Z  DB inst~nce with ~utom~tic~lly sc~ling re~d replic~s. Cre~te ~n ;;m~zon  EventBridge rule th~t invokes ~n ;;WS  L~mbd~ function to cre~te ~ l~rger re~d replic~ before ~ s~le event.  F~il over to the l~rger re~d replic~. Cre~te ~nother  EventBridge rule th~t invokes ~nother  L~mbd~ function to sc~le down the re~d replic~ ~fter the s~le event.
  C. Use ~ predictive sc~ling policy for the  EC2 inst~nces.  Host the d~t~b~se on ~n ;;m~zon  RDS for  PostgreSQL  Multi;;Z  DB inst~nce with ~utom~tic~lly sc~ling re~d replic~s. Cre~te ~n ;;WS Step  Functions st~te m~chine to run p~r~llel ;;WS  L~mbd~ functions to pre-w~rm the d~t~b~se before ~ s~le event. Cre~te ~n ;;m~zon  EventBridge rule to invoke the st~te m~chine.
  D. Use ~ scheduled sc~ling policy for the  EC2 inst~nces.  Host the d~t~b~se on ~n ;;m~zon ;;uror~  PostgreSQL  Multi-;;Z  DB cluster. Cre~te ~n ;;m~zon  EventBridge rule th~t invokes ~n ;;WS  L~mbd~ function to cre~te ~ l~rger ;;uror~  Replic~ before ~ s~le event.  F~il over to the l~rger ;;uror~  Replic~. Cre~te ~nother  EventBridge rule th~t invokes ~nother  L~mbd~ function to sc~le down the ;;uror~  Replic~ ~fter the s~le event.

 Correct ;;nswer: B
 D (100%)

 Question #375
 ;; comp~ny runs ~n intr~net ~pplic~tion on premises. The comp~ny w~nts to con gure ~ cloud b~ckup of the ~pplic~tion. The comp~ny h~s selected ;;WS  El~stic  Dis~ster  Recovery for this solution. The comp~ny requires th~t replic~tion tr~ c does not tr~vel through the public internet. The ~pplic~tion ~lso must not be ~ccessible from the internet. The comp~ny does not w~nt this solution to consume ~ll ~v~il~ble network b~ndwidth bec~use other ~pplic~tions require b~ndwidth. Which combin~tion of steps will meet these requirements? (Choose three.)
  ;;. Cre~te ~ VPC th~t h~s ~t le~st two priv~te subnets, two  N;;T g~tew~ys, ~nd ~ virtu~l priv~te g~tew~y.
  B. Cre~te ~ VPC th~t h~s ~t le~st two public subnets, ~ virtu~l priv~te g~tew~y, ~nd ~n internet g~tew~y.
  C. Cre~te ~n ;;WS Site-to-Site VPN connection between the on-premises network ~nd the t~rget ;;WS network.
  D. Cre~te ~n ;;WS  Direct Connect connection ~nd ~  Direct Connect g~tew~y between the on-premises network ~nd the t~rget ;;WS network.
  E.  During con gur~tion of the replic~tion servers, select the option to use priv~te  IP ~ddresses for d~t~ replic~tion.
  F.  During con gur~tion of the l~unch settings for the t~rget servers, select the option to ensure th~t the  Recovery inst~nce’s priv~te  IP ~ddress m~tches the source server's priv~te  IP ~ddress.

 Correct ;;nswer: ;;EF
 ;;DE (63%)                         13%        13%       6%

 Question #376
 ;; comp~ny th~t provides im~ge stor~ge services w~nts to deploy ~ customer-f~cing solution to ;;WS.  Millions of individu~l customers will use the solution. The solution will receive b~tches of l~rge im~ge  les, resize the  les, ~nd store the  les in ~n ;;m~zon S3 bucket for up to 6 months. The solution must h~ndle signi c~nt v~ri~nce in dem~nd. The solution must ~lso be reli~ble ~t enterprise sc~le ~nd h~ve the ~bility to rerun processing jobs in the event of f~ilure. Which solution will meet these requirements  MOST cost-effectively?
  ;;. Use ;;WS Step  Functions to process the S3 event th~t occurs when ~ user stores ~n im~ge.  Run ~n ;;WS  L~mbd~ function th~t resizes the im~ge in pl~ce ~nd repl~ces the origin~l  le in the S3 bucket. Cre~te ~n S3  Lifecycle expir~tion policy to expire ~ll stored im~ges ~fter 6 months.
  B. Use ;;m~zon  EventBridge to process the S3 event th~t occurs when ~ user uplo~ds ~n im~ge.  Run ~n ;;WS  L~mbd~ function th~t resizes the im~ge in pl~ce ~nd repl~ces the origin~l  le in the S3 bucket. Cre~te ~n S3  Lifecycle expir~tion policy to expire ~ll stored im~ges ~fter 6 months.
  C. Use S3  Event  Noti c~tions to invoke ~n ;;WS  L~mbd~ function when ~ user stores ~n im~ge. Use the  L~mbd~ function to resize the im~ge in pl~ce ~nd to store the origin~l  le in the S3 bucket. Cre~te ~n S3  Lifecycle policy to move ~ll stored im~ges to S3 St~nd~rd-Infrequent ;;ccess (S3 St~nd~rd-I;;) ~fter 6 months.
  D. Use ;;m~zon Simple Queue Service (;;m~zon SQS) to process the S3 event th~t occurs when ~ user stores ~n im~ge.  Run ~n ;;WS  L~mbd~ function th~t resizes the im~ge ~nd stores the resized  le in ~n S3 bucket th~t uses S3 St~nd~rd-Infrequent ;;ccess (S3 St~nd~rd-I;;). Cre~te ~n S3  Lifecycle policy to move ~ll stored im~ges to S3 Gl~cier  Deep ;;rchive ~fter 6 months.

 Correct ;;nswer: D
 B (34%)                    ;; (31%)               D (24%)          7%

 Question #377
 ;; comp~ny h~s ~n org~niz~tion in ;;WS Org~niz~tions th~t includes ~ sep~r~te ;;WS ~ccount for e~ch of the comp~ny’s dep~rtments. ;;pplic~tion te~ms from different dep~rtments develop ~nd deploy solutions independently. The comp~ny w~nts to reduce compute costs ~nd m~n~ge costs ~ppropri~tely ~cross dep~rtments. The comp~ny ~lso w~nts to improve visibility into billing for individu~l dep~rtments. The comp~ny does not w~nt to lose oper~tion~l  exibility when the comp~ny selects compute resources. Which solution will meet these requirements?
  ;;. Use ;;WS  Budgets for e~ch dep~rtment. Use T~g  Editor to ~pply t~gs to ~ppropri~te resources.  Purch~se  EC2  Inst~nce S~vings  Pl~ns.
  B. Con gure ;;WS Org~niz~tions to use consolid~ted billing.  Implement ~ t~gging str~tegy th~t identi es dep~rtments. Use SCPs to ~pply t~gs to ~ppropri~te resources.  Purch~se  EC2  Inst~nce S~vings  Pl~ns.
  C. Con gure ;;WS Org~niz~tions to use consolid~ted billing.  Implement ~ t~gging str~tegy th~t identi es dep~rtments. Use T~g  Editor to ~pply t~gs to ~ppropri~te resources.  Purch~se Compute S~vings  Pl~ns.
  D. Use ;;WS  Budgets for e~ch dep~rtment. Use SCPs to ~pply t~gs to ~ppropri~te resources.  Purch~se Compute S~vings  Pl~ns.

 Correct ;;nswer: C
 C (82%)                                 B (18%)

 Question #378
 ;; comp~ny h~s ~ web ~pplic~tion th~t securely uplo~ds pictures ~nd videos to ~n ;;m~zon S3 bucket. The comp~ny requires th~t only ~uthentic~ted users ~re ~llowed to post content. The ~pplic~tion gener~tes ~ presigned URL th~t is used to uplo~d objects through ~ browser interf~ce.  Most users ~re reporting slow uplo~d times for objects l~rger th~n  100  MB. Wh~t c~n ~ solutions ~rchitect do to improve the perform~nce of these uplo~ds while ensuring only ~uthentic~ted users ~re ~llowed to post content?
  ;;. Set up ~n ;;m~zon ;;PI G~tew~y with ~n edge-optimized ;;PI endpoint th~t h~s ~ resource ~s ~n S3 service proxy. Con gure the  PUT method for this resource to expose the S3  PutObject oper~tion. Secure the ;;PI G~tew~y using ~ COGNITO_USER_POOLS ~uthorizer.  H~ve the browser interf~ce use ;;PI G~tew~y inste~d of the presigned URL to uplo~d objects.
  B. Set up ~n ;;m~zon ;;PI G~tew~y with ~ region~l ;;PI endpoint th~t h~s ~ resource ~s ~n S3 service proxy. Con gure the  PUT method for this resource to expose the S3  PutObject oper~tion. Secure the ;;PI G~tew~y using ~n ;;WS  L~mbd~ ~uthorizer.  H~ve the browser interf~ce use ;;PI G~tew~y inste~d of the presigned URL to uplo~d objects.
  C.  En~ble ~n S3 Tr~nsfer ;;cceler~tion endpoint on the S3 bucket. Use the endpoint when gener~ting the presigned URL.  H~ve the browser interf~ce uplo~d the objects to this URL using the S3 multip~rt uplo~d ;;PI.
  D. Con gure ~n ;;m~zon CloudFront distribution for the destin~tion S3 bucket.  En~ble  PUT ~nd  POST methods for the CloudFront c~che beh~vior. Upd~te the CloudFront origin to use ~n origin ~ccess identity (O;;I). Give the O;;I user 3:  PutObject permissions in the bucket policy. H~ve the browser interf~ce uplo~d objects using the CloudFront distribution.

 Correct ;;nswer: B
 C (71%)                                 ;; (29%)

 Question #379
 ;; l~rge comp~ny is migr~ting its entire  IT portfolio to ;;WS.  E~ch business unit in the comp~ny h~s ~ st~nd~lone ;;WS ~ccount th~t supports both development ~nd test environments.  New ~ccounts to support production worklo~ds will be needed soon. The  n~nce dep~rtment requires ~ centr~lized method for p~yment but must m~int~in visibility into e~ch group's spending to ~lloc~te costs. The security te~m requires ~ centr~lized mech~nism to control  I;;M us~ge in ~ll the comp~ny’s ~ccounts. Wh~t combin~tion of the following options meets the comp~ny’s needs with the  LE;;ST effort? (Choose two.)
  ;;. Use ~ collection of p~r~meterized ;;WS CloudForm~tion templ~tes de ning common  I;;M permissions th~t ~re l~unched into e~ch ~ccount. Require ~ll new ~nd existing ~ccounts to l~unch the ~ppropri~te st~cks to enforce the le~st privilege model.
  B. Use ;;WS Org~niz~tions to cre~te ~ new org~niz~tion from ~ chosen p~yer ~ccount ~nd de ne ~n org~niz~tion~l unit hier~rchy.  Invite the existing ~ccounts to join the org~niz~tion ~nd cre~te new ~ccounts using Org~niz~tions.
  C.  Require e~ch business unit to use its own ;;WS ~ccounts. T~g e~ch ;;WS ~ccount ~ppropri~tely ~nd en~ble Cost  Explorer to ~dminister ch~rgeb~cks.
  D.  En~ble ~ll fe~tures of ;;WS Org~niz~tions ~nd est~blish ~ppropri~te service control policies th~t  lter  I;;M permissions for sub-~ccounts.
  E. Consolid~te ~ll of the comp~ny's ;;WS ~ccounts into ~ single ;;WS ~ccount. Use t~gs for billing purposes ~nd the  I;;M’s ;;ccess ;;dvisor fe~ture to enforce the le~st privilege model.

 Correct ;;nswer: ;;B
 BD (100%)

 Question #380
 ;; comp~ny h~s ~ solution th~t ~n~lyzes we~ther d~t~ from thous~nds of we~ther st~tions. The we~ther st~tions send the d~t~ over ~n ;;m~zon ;;PI G~tew~y  REST ;;PI th~t h~s ~n ;;WS  L~mbd~ function integr~tion. The  L~mbd~ function c~lls ~ third-p~rty service for d~t~ pre-processing. The third-p~rty service gets overlo~ded ~nd f~ils the pre-processing, c~using ~ loss of d~t~. ;; solutions ~rchitect must improve the resiliency of the solution. The solutions ~rchitect must ensure th~t no d~t~ is lost ~nd th~t d~t~ c~n be processed l~ter if f~ilures occur. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Cre~te ~n ;;m~zon Simple Queue Service (;;m~zon SQS) queue. Con gure the queue ~s the de~d-letter queue for the ;;PI.
  B. Cre~te two ;;m~zon Simple Queue Service (;;m~zon SQS) queues: ~ prim~ry queue ~nd ~ second~ry queue. Con gure the second~ry queue ~s the de~d-letter queue for the prim~ry queue. Upd~te the ;;PI to use ~ new integr~tion to the prim~ry queue. Con gure the  L~mbd~ function ~s the invoc~tion t~rget for the prim~ry queue.
  C. Cre~te two ;;m~zon  EventBridge event buses: ~ prim~ry event bus ~nd ~ second~ry event bus. Upd~te the ;;PI to use ~ new integr~tion to the prim~ry event bus. Con gure ~n  EventBridge rule to re~ct to ~ll events on the prim~ry event bus. Specify the  L~mbd~ function ~s the t~rget of the rule. Con gure the second~ry event bus ~s the f~ilure destin~tion for the  L~mbd~ function.
  D. Cre~te ~ custom ;;m~zon  EventBridge event bus. Con gure the event bus ~s the f~ilure destin~tion for the  L~mbd~ function.

 Correct ;;nswer: B
 B (92%)                                    8%

 Question #381
 ;; comp~ny built ~n ecommerce website on ;;WS using ~ three-tier web ~rchitecture. The ~pplic~tion is J~v~-b~sed ~nd composed of ~n ;;m~zon CloudFront distribution, ~n ;;p~che web server l~yer of ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group, ~nd ~ b~ckend ;;m~zon ;;uror~  MySQL d~t~b~se. L~st month, during ~ promotion~l s~les event, users reported errors ~nd timeouts while ~dding items to their shopping c~rts. The oper~tions te~m recovered the logs cre~ted by the web servers ~nd reviewed ;;uror~  DB cluster perform~nce metrics. Some of the web servers were termin~ted before logs could be collected ~nd the ;;uror~ metrics were not su cient for query perform~nce ~n~lysis. Which combin~tion of steps must the solutions ~rchitect t~ke to improve ~pplic~tion perform~nce visibility during pe~k tr~ c events? (Choose three.)
  ;;. Con gure the ;;uror~  MySQL  DB cluster to publish slow query ~nd error logs to ;;m~zon CloudW~tch  Logs.
  B.  Implement the ;;WS X-R~y SDK to tr~ce incoming  HTTP requests on the  EC2 inst~nces ~nd implement tr~cing of SQL queries with the X-R~y SDK for J~v~.
  C. Con gure the ;;uror~  MySQL  DB cluster to stre~m slow query ~nd error logs to ;;m~zon  Kinesis.
  D.  Inst~ll ~nd con gure ~n ;;m~zon CloudW~tch  Logs ~gent on the  EC2 inst~nces to send the ;;p~che logs to CloudW~tch  Logs.
  E.  En~ble ~nd con gure ;;WS CloudTr~il to collect ~nd ~n~lyze ~pplic~tion ~ctivity from ;;m~zon  EC2 ~nd ;;uror~
  F.  En~ble ;;uror~  MySQL  DB cluster perform~nce benchm~rking ~nd publish the stre~m to ;;WS X-R~y.

 Correct ;;nswer: ;;EF
 ;;BD (100%)

 Question #382
 ;; comp~ny th~t provisions job bo~rds for ~ se~son~l workforce is seeing ~n incre~se in tr~ c ~nd us~ge. The b~ckend services run on ~ p~ir of ;;m~zon  EC2 inst~nces behind ~n ;;pplic~tion  Lo~d  B~l~ncer with ;;m~zon  Dyn~moDB ~s the d~t~store. ;;pplic~tion re~d ~nd write tr~ c is slow during pe~k se~sons. Which option provides ~ sc~l~ble ~pplic~tion ~rchitecture to h~ndle pe~k se~sons with the  LE;;ST development effort?
  ;;.  Migr~te the b~ckend services to ;;WS  L~mbd~.  Incre~se the re~d ~nd write c~p~city of  Dyn~moDB.
  B.  Migr~te the b~ckend services to ;;WS  L~mbd~. Con gure  Dyn~moDB to use glob~l t~bles.
  C. Use ;;uto Sc~ling groups for the b~ckend services. Use  Dyn~moDB ~uto sc~ling.
  D. Use ;;uto Sc~ling groups for the b~ckend services. Use ;;m~zon Simple Queue Service (;;m~zon SQS) ~nd ~n ;;WS  L~mbd~ function to write to  Dyn~moDB.

 Correct ;;nswer: B
 C (100%)

 Question #383
 ;; comp~ny is migr~ting to the cloud.  It w~nts to ev~lu~te the con gur~tions of virtu~l m~chines in its existing d~t~ center environment to ensure th~t it c~n size new ;;m~zon  EC2 inst~nces ~ccur~tely. The comp~ny w~nts to collect metrics, such ~s CPU, memory, ~nd disk utiliz~tion, ~nd it needs ~n inventory of wh~t processes ~re running on e~ch inst~nce. The comp~ny would ~lso like to monitor network connections to m~p communic~tions between servers. Which would en~ble the collection of this d~t~  MOST cost effectively?
  ;;. Use ;;WS ;;pplic~tion  Discovery Service ~nd deploy the d~t~ collection ~gent to e~ch virtu~l m~chine in the d~t~ center.
  B. Con gure the ;;m~zon CloudW~tch ~gent on ~ll servers within the loc~l environment ~nd publish metrics to ;;m~zon CloudW~tch  Logs.
  C. Use ;;WS ;;pplic~tion  Discovery Service ~nd en~ble ~gentless discovery in the existing virtu~liz~tion environment.
  D.  En~ble ;;WS ;;pplic~tion  Discovery Service in the ;;WS  M~n~gement Console ~nd con gure the corpor~te  rew~ll to ~llow sc~ns over ~ VPN.

 Correct ;;nswer: D
 ;; (90%)                                    5%

 Question #384
 ;; comp~ny provides ~ softw~re ~s ~ service (S~~S) ~pplic~tion th~t runs in the ;;WS Cloud. The ~pplic~tion runs on ;;m~zon  EC2 inst~nces behind ~  Network  Lo~d  B~l~ncer (NLB). The inst~nces ~re in ~n ;;uto Sc~ling group ~nd ~re distributed ~cross three ;;v~il~bility Zones in ~ single ;;WS Region. The comp~ny is deploying the ~pplic~tion into ~ddition~l  Regions. The comp~ny must provide st~tic  IP ~ddresses for the ~pplic~tion to customers so th~t the customers c~n ~dd the  IP ~ddresses to ~llow lists. The solution must ~utom~tic~lly route customers to the  Region th~t is geogr~phic~lly closest to them. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;m~zon CloudFront distribution. Cre~te ~ CloudFront origin group. ;;dd the  NLB for e~ch ~ddition~l  Region to the origin group. Provide customers with the  IP ~ddress r~nges of the distribution’s edge loc~tions.
  B. Cre~te ~n ;;WS Glob~l ;;cceler~tor st~nd~rd ~cceler~tor. Cre~te ~ st~nd~rd ~cceler~tor endpoint for the  NLB in e~ch ~ddition~l  Region. Provide customers with the Glob~l ;;cceler~tor  IP ~ddress.
  C. Cre~te ~n ;;m~zon CloudFront distribution. Cre~te ~ custom origin for the  NLB in e~ch ~ddition~l  Region.  Provide customers with the  IP ~ddress r~nges of the distribution’s edge loc~tions.
  D. Cre~te ~n ;;WS Glob~l ;;cceler~tor custom routing ~cceler~tor. Cre~te ~ listener for the custom routing ~cceler~tor. ;;dd the  IP ~ddress ~nd ports for the  NLB in e~ch ~ddition~l  Region.  Provide customers with the Glob~l ;;cceler~tor  IP ~ddress.

 Correct ;;nswer: C
 B (85%)                                  D (15%)

 Question #385
 ;; comp~ny is running multiple worklo~ds in the ;;WS Cloud. The comp~ny h~s sep~r~te units for softw~re development. The comp~ny uses ;;WS Org~niz~tions ~nd feder~tion with S;;ML to give permissions to developers to m~n~ge resources in their ;;WS ~ccounts. The development units e~ch deploy their production worklo~ds into ~ common production ~ccount. Recently, ~n incident occurred in the production ~ccount in which members of ~ development unit termin~ted ~n  EC2 inst~nce th~t belonged to ~ different development unit. ;; solutions ~rchitect must cre~te ~ solution th~t prevents ~ simil~r incident from h~ppening in the future. The solution ~lso must ~llow developers the possibility to m~n~ge the inst~nces used for their worklo~ds. Which str~tegy will meet these requirements?
  ;;. Cre~te sep~r~te OUs in ;;WS Org~niz~tions for e~ch development unit. ;;ssign the cre~ted OUs to the comp~ny ;;WS ~ccounts. Cre~te sep~r~te SCP with ~ deny ~ction ~nd ~ StringNotEqu~ls condition for the  DevelopmentUnit resource t~g th~t m~tches the development unit n~me. ;;ssign the SCP to the corresponding OU.
  B.  P~ss ~n ~ttribute for  DevelopmentUnit ~s ~n ;;WS Security Token Service (;;WS STS) session t~g during S;;ML feder~tion. Upd~te the  I;;M policy for the developers’ ~ssumed  I;;M role with ~ deny ~ction ~nd ~ StringNotEqu~ls condition for the  DevelopmentUnit resource t~g ~nd ~ws:Princip~lT~g/DevelopmentUnit.
  C.  P~ss ~n ~ttribute for  DevelopmentUnit ~s ~n ;;WS Security Token Service (;;WS STS) session t~g during S;;ML feder~tion. Cre~te ~n SCP with ~n ~llow ~ction ~nd ~ StringEqu~ls condition for the  DevelopmentUnit resource t~g ~nd ~ws:Princip~lT~g/DevelopmentUnit. ;;ssign the SCP to the root OU.
  D. Cre~te sep~r~te  I;;M policies for e~ch development unit.  For every  I;;M policy, ~dd ~n ~llow ~ction ~nd ~ StringEqu~ls condition for the DevelopmentUnit resource t~g ~nd the development unit n~me.  During S;;ML feder~tion, use ;;WS Security Token Service (;;WS STS) to ~ssign the  I;;M policy ~nd m~tch the development unit n~me to the ~ssumed  I;;M role.

 Correct ;;nswer: B
 B (73%)                                  ;; (27%)

 Question #386
 ;;n enterprise comp~ny is building ~n infr~structure services pl~tform for its users. The comp~ny h~s the following requirements: •  Provide le~st privilege ~ccess to users when l~unching ;;WS infr~structure so users c~nnot provision un~pproved services. • Use ~ centr~l ~ccount to m~n~ge the cre~tion of infr~structure services. •  Provide the ~bility to distribute infr~structure services to multiple ~ccounts in ;;WS Org~niz~tions. •  Provide the ~bility to enforce t~gs on ~ny infr~structure th~t is st~rted by users. Which combin~tion of ~ctions using ;;WS services will meet these requirements? (Choose three.)
  ;;.  Develop infr~structure services using ;;WS CloudForm~tion templ~tes. ;;dd the templ~tes to ~ centr~l ;;m~zon S3 bucket ~nd ~dd the  I;;M roles or users th~t require ~ccess to the S3 bucket policy.
  B.  Develop infr~structure services using ;;WS CloudForm~tion templ~tes. Uplo~d e~ch templ~te ~s ~n ;;WS Service C~t~log product to portfolios cre~ted in ~ centr~l ;;WS ~ccount. Sh~re these portfolios with the Org~niz~tions structure cre~ted for the comp~ny.
  C. ;;llow user  I;;M roles to h~ve ;;WSCloudForm~tionFull;;ccess ~nd ;;m~zonS3Re~dOnly;;ccess permissions. ;;dd ~n Org~niz~tions SCP ~t the ;;WS ~ccount root user level to deny ~ll services except ;;WS CloudForm~tion ~nd ;;m~zon S3.
  D. ;;llow user  I;;M roles to h~ve ServiceC~t~logEndUser;;ccess permissions only. Use ~n ~utom~tion script to import the centr~l portfolios to loc~l ;;WS ~ccounts, copy the T~gOption, ~ssign users ~ccess, ~nd ~pply l~unch constr~ints.
  E. Use the ;;WS Service C~t~log T~gOption  Libr~ry to m~int~in ~ list of t~gs required by the comp~ny. ;;pply the T~gOption to ;;WS Service C~t~log products or portfolios.
  F. Use the ;;WS CloudForm~tion  Resource T~gs property to enforce the ~pplic~tion of t~gs to ~ny CloudForm~tion templ~tes th~t will be cre~ted for users.

 Correct ;;nswer: BDE
 BDE (92%)                                   8%

 Question #387
 ;; comp~ny deploys ~ new web ~pplic~tion. ;;s p~rt of the setup, the comp~ny con gures ;;WS W;;F to log to ;;m~zon S3 through ;;m~zon  Kinesis D~t~  Firehose. The comp~ny develops ~n ;;m~zon ;;then~ query th~t runs once d~ily to return ;;WS W;;F log d~t~ from the previous 24 hours. The volume of d~ily logs is const~nt.  However, over time, the s~me query is t~king more time to run. ;; solutions ~rchitect needs to design ~ solution to prevent the query time from continuing to incre~se. The solution must minimize oper~tion~l overhe~d. Which solution will meet these requirements?
  ;;. Cre~te ~n ;;WS  L~mbd~ function th~t consolid~tes e~ch d~y's ;;WS W;;F logs into one log  le.
  B.  Reduce the ~mount of d~t~ sc~nned by con guring ;;WS W;;F to send logs to ~ different S3 bucket e~ch d~y.
  C. Upd~te the  Kinesis  D~t~  Firehose con gur~tion to p~rtition the d~t~ in ;;m~zon S3 by d~te ~nd time. Cre~te extern~l t~bles for ;;m~zon Redshift. Con gure ;;m~zon  Redshift Spectrum to query the d~t~ source.
  D.  Modify the  Kinesis  D~t~  Firehose con gur~tion ~nd ;;then~ t~ble de nition to p~rtition the d~t~ by d~te ~nd time. Ch~nge the ;;then~ query to view the relev~nt p~rtitions.

 Correct ;;nswer: D
 D (100%)

 Question #388
 ;; comp~ny is developing ~ web ~pplic~tion th~t runs on ;;m~zon  EC2 inst~nces in ~n ;;uto Sc~ling group behind ~ public-f~cing ;;pplic~tion  Lo~d B~l~ncer (;;LB). Only users from ~ speci c country ~re ~llowed to ~ccess the ~pplic~tion. The comp~ny needs the ~bility to log the ~ccess requests th~t h~ve been blocked. The solution should require the le~st possible m~inten~nce. Which solution meets these requirements?
  ;;. Cre~te ~n  IPSet cont~ining ~ list of  IP r~nges th~t belong to the speci ed country. Cre~te ~n ;;WS W;;F web ;;CL. Con gure ~ rule to block ~ny requests th~t do not origin~te from ~n  IP r~nge in the  IPSet. ;;ssoci~te the rule with the web ;;CL. ;;ssoci~te the web ;;CL with the ;;LB.
  B. Cre~te ~n ;;WS W;;F web ;;CL. Con gure ~ rule to block ~ny requests th~t do not origin~te from the speci ed country. ;;ssoci~te the rule with the web ;;CL. ;;ssoci~te the web ;;CL with the ;;LB.
  C. Con gure ;;WS Shield to block ~ny requests th~t do not origin~te from the speci ed country. ;;ssoci~te ;;WS Shield with the ;;LB.
  D. Cre~te ~ security group rule th~t ~llows ports 80 ~nd 443 from  IP r~nges th~t belong to the speci ed country. ;;ssoci~te the security group with the ;;LB.

 Correct ;;nswer: C
 B (100%)

 Question #389
 ;; comp~ny is migr~ting ~n ~pplic~tion from on-premises infr~structure to the ;;WS Cloud.  During migr~tion design meetings, the comp~ny expressed concerns ~bout the ~v~il~bility ~nd recovery options for its leg~cy Windows  le server. The  le server cont~ins sensitive business- critic~l d~t~ th~t c~nnot be recre~ted in the event of d~t~ corruption or d~t~ loss. ;;ccording to compli~nce requirements, the d~t~ must not tr~vel ~cross the public internet. The comp~ny w~nts to move to ;;WS m~n~ged services where possible. The comp~ny decides to store the d~t~ in ~n ;;m~zon  FSx for Windows  File Server  le system. ;; solutions ~rchitect must design ~ solution th~t copies the d~t~ to ~nother ;;WS  Region for dis~ster recovery (DR) purposes. Which solution will meet these requirements?
  ;;. Cre~te ~ destin~tion ;;m~zon S3 bucket in the  DR  Region.  Est~blish connectivity between the  FSx for Windows  File Server  le system in the prim~ry  Region ~nd the S3 bucket in the  DR  Region by using ;;m~zon  FSx  File G~tew~y. Con gure the S3 bucket ~s ~ continuous b~ckup source in  FSx  File G~tew~y.
  B. Cre~te ~n  FSx for Windows  File Server  le system in the  DR  Region.  Est~blish connectivity between the VPC the prim~ry  Region ~nd the VPC in the  DR  Region by using ;;WS Site-to-Site VPN. Con gure ;;WS  D~t~Sync to communic~te by using VPN endpoints.
  C. Cre~te ~n  FSx for Windows  File Server  le system in the  DR  Region.  Est~blish connectivity between the VPC in the prim~ry  Region ~nd the VPC in the  DR  Region by using VPC peering. Con gure ;;WS  D~t~Sync to communic~te by using interf~ce VPC endpoints with ;;WS Priv~teLink.
  D. Cre~te ~n  FSx for Windows  File Server  le system in the  DR  Region.  Est~blish connectivity between the VPC in the prim~ry  Region ~nd the VPC in the  DR  Region by using ;;WS Tr~nsit G~tew~y in e~ch  Region. Use ;;WS Tr~nsfer  F~mily to copy  les between the  FSx for Windows  File Server  le system in the prim~ry  Region ~nd the  FSx for Windows  File Server  le system in the  DR  Region over the priv~te ;;WS b~ckbone network.

 Correct ;;nswer: C
 C (91%)                                    9%

 Question #390
 ;; comp~ny is currently in the design ph~se of ~n ~pplic~tion th~t will need ~n  RPO of less th~n 5 minutes ~nd ~n  RTO of less th~n  10 minutes. The solutions ~rchitecture te~m is forec~sting th~t the d~t~b~se will store ~pproxim~tely  10 TB of d~t~. ;;s p~rt of the design, they ~re looking for ~ d~t~b~se solution th~t will provide the comp~ny with the ~bility to f~il over to ~ second~ry  Region. Which solution will meet these business requirements ~t the  LOWEST cost?
  ;;.  Deploy ~n ;;m~zon ;;uror~  DB cluster ~nd t~ke sn~pshots of the cluster every 5 minutes. Once ~ sn~pshot is complete, copy the sn~pshot to ~ second~ry  Region to serve ~s ~ b~ckup in the event of ~ f~ilure.
  B.  Deploy ~n ;;m~zon  RDS inst~nce with ~ cross-Region re~d replic~ in ~ second~ry  Region.  In the event of ~ f~ilure, promote the re~d replic~ to become the prim~ry.
  C.  Deploy ~n ;;m~zon ;;uror~  DB cluster in the prim~ry  Region ~nd ~nother in ~ second~ry  Region. Use ;;WS  DMS to keep the second~ry  Region in sync.
  D.  Deploy ~n ;;m~zon  RDS inst~nce with ~ re~d replic~ in the s~me  Region.  In the event of ~ f~ilure, promote the re~d replic~ to become the prim~ry.

 Correct ;;nswer: B
 B (82%)                                   C (18%)

 Question #391
 ;;  n~nci~l comp~ny needs to cre~te ~ sep~r~te ;;WS ~ccount for ~ new digit~l w~llet ~pplic~tion. The comp~ny uses ;;WS Org~niz~tions to m~n~ge its ~ccounts. ;; solutions ~rchitect uses the  I;;M user Support1 from the m~n~gement ~ccount to cre~te ~ new member ~ccount with  n~nce1@ex~mple.com ~s the em~il ~ddress. Wh~t should the solutions ~rchitect do to cre~te  I;;M users in the new member ~ccount?
  ;;. Sign in to the ;;WS  M~n~gement Console with ;;WS ~ccount root user credenti~ls by using the 64-ch~r~cter p~ssword from the initi~l ;;WS Org~niz~tions em~il sent to  n~nce1@ex~mple.com. Set up the  I;;M users ~s required.
  B.  From the m~n~gement ~ccount, switch roles to ~ssume the Org~niz~tion;;ccount;;ccessRole role with the ~ccount  ID of the new member ~ccount. Set up the  I;;M users ~s required.
  C. Go to the ;;WS  M~n~gement Console sign-in p~ge. Choose “Sign in using root ~ccount credenti~ls.” Sign in in by using the em~il ~ddress  n~nce  1@ex~mple.com ~nd the m~n~gement ~ccount's root p~ssword. Set up the  I;;M users ~s required.
  D. Go to the ;;WS  M~n~gement Console sign-in p~ge. Sign in by using the ~ccount  ID of the new member ~ccount ~nd the Support1  I;;M credenti~ls. Set up the  I;;M users ~s required.

 Correct ;;nswer: ;;
 B (73%)                                  D (27%)

 Question #392
 ;; c~r rent~l comp~ny h~s built ~ serverless  REST ;;PI to provide d~t~ to its mobile ~pp. The ~pp consists of ~n ;;m~zon ;;PI G~tew~y ;;PI with ~ Region~l endpoint, ;;WS  L~mbd~ functions, ~nd ~n ;;m~zon ;;uror~  MySQL Serverless  DB cluster. The comp~ny recently opened the ;;PI to mobile ~pps of p~rtners. ;; signi c~nt incre~se in the number of requests resulted, c~using spor~dic d~t~b~se memory errors. ;;n~lysis of the ;;PI tr~ c indic~tes th~t clients ~re m~king multiple  HTTP GET requests for the s~me queries in ~ short period of time. Tr~ c is concentr~ted during business hours, with spikes ~round holid~ys ~nd other events. The comp~ny needs to improve its ~bility to support the ~ddition~l us~ge while minimizing the incre~se in costs ~ssoci~ted with the solution. Which str~tegy meets these requirements?
  ;;. Convert the ;;PI G~tew~y  Region~l endpoint to ~n edge-optimized endpoint.  En~ble c~ching in the production st~ge.
  B.  Implement ~n ;;m~zon  El~stiC~che for  Redis c~che to store the results of the d~t~b~se c~lls.  Modify the  L~mbd~ functions to use the c~che.
  C.  Modify the ;;uror~ Serverless  DB cluster con gur~tion to incre~se the m~ximum ~mount of ~v~il~ble memory.
  D.  En~ble throttling in the ;;PI G~tew~y production st~ge. Set the r~te ~nd burst v~lues to limit the incoming c~lls.

 Correct ;;nswer: C
 ;; (59%)                                   B (41%)

 Question #393
 ;; comp~ny is migr~ting ~n on-premises ~pplic~tion ~nd ~  MySQL d~t~b~se to ;;WS. The ~pplic~tion processes highly sensitive d~t~, ~nd new d~t~ is const~ntly upd~ted in the d~t~b~se. The d~t~ must not be tr~nsferred over the internet. The comp~ny ~lso must encrypt the d~t~ in tr~nsit ~nd ~t rest. The d~t~b~se is 5 TB in size. The comp~ny ~lre~dy h~s cre~ted the d~t~b~se schem~ in ~n ;;m~zon  RDS for  MySQL  DB inst~nce. The comp~ny h~s set up ~  1 Gbps ;;WS  Direct Connect connection to ;;WS. The comp~ny ~lso h~s set up ~ public VIF ~nd ~ priv~te VIF. ;; solutions ~rchitect needs to design ~ solution th~t will migr~te the d~t~ to ;;WS with the le~st possible downtime. Which solution will meet these requirements?
  ;;.  Perform ~ d~t~b~se b~ckup. Copy the b~ckup  les to ~n ;;WS Snowb~ll  Edge Stor~ge Optimized device.  Import the b~ckup to ;;m~zon S3. Use server-side encryption with ;;m~zon S3 m~n~ged encryption keys (SSE-S3) for encryption ~t rest. Use TLS for encryption in tr~nsit.  Import the d~t~ from ;;m~zon S3 to the  DB inst~nce.
  B. Use ;;WS  D~t~b~se  Migr~tion Service (;;WS  DMS) to migr~te the d~t~ to ;;WS. Cre~te ~  DMS replic~tion inst~nce in ~ priv~te subnet. Cre~te VPC endpoints for ;;WS  DMS. Con gure ~  DMS t~sk to copy d~t~ from the on-premises d~t~b~se to the  DB inst~nce by using full lo~d plus ch~nge d~t~ c~pture (CDC). Use the ;;WS  Key  M~n~gement Service (;;WS  KMS) def~ult key for encryption ~t rest. Use TLS for encryption in tr~nsit.
  C.  Perform ~ d~t~b~se b~ckup. Use ;;WS  D~t~Sync to tr~nsfer the b~ckup  les to ;;m~zon S3. Use server-side encryption with ;;m~zon S3 m~n~ged encryption keys (SSE-S3) for encryption ~t rest. Use TLS for encryption in tr~nsit.  Import the d~t~ from ;;m~zon S3 to the  DB inst~nce.
  D. Use ;;m~zon S3  File G~tew~y. Set up ~ priv~te connection to ;;m~zon S3 by using ;;WS  Priv~teLink.  Perform ~ d~t~b~se b~ckup. Copy the b~ckup  les to ;;m~zon S3. Use server-side encryption with ;;m~zon S3 m~n~ged encryption keys (SSE-S3) for encryption ~t rest. Use TLS for encryption in tr~nsit.  Import the d~t~ from ;;m~zon S3 to the  DB inst~nce.

 Correct ;;nswer: C
 B (100%)

 Question #394
 ;;ccomp~ny is deploying ~ new cluster for big d~t~ ~n~lytics on ;;WS. The cluster will run ~cross m~ny  Linux ;;m~zon  EC2 inst~nces th~t ~re spre~d ~cross multiple ;;v~il~bility Zones. ;;ll of the nodes in the cluster must h~ve re~d ~nd write ~ccess to common underlying  le stor~ge. The  le stor~ge must be highly ~v~il~ble, must be resilient, must be comp~tible with the  Port~ble Oper~ting System  Interf~ce (POSIX), ~nd must ~ccommod~te high levels of throughput. Which stor~ge solution will meet these requirements?
  ;;.  Provision ~n ;;WS Stor~ge G~tew~y  le g~tew~y  NFS  le sh~re th~t is ~tt~ched to ~n ;;m~zon S3 bucket.  Mount the  NFS  le sh~re on e~ch EC2 inst~nce in the cluster.
  B.  Provision ~ new ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system th~t uses Gener~l  Purpose perform~nce mode.  Mount the  EFS  le system on e~ch  EC2 inst~nce in the cluster.
  C.  Provision ~ new ;;m~zon  El~stic  Block Store (;;m~zon  EBS) volume th~t uses the io2 volume type. ;;tt~ch the  EBS volume to ~ll of the  EC2 inst~nces in the cluster.
  D.  Provision ~ new ;;m~zon  El~stic  File System (;;m~zon  EFS)  le system th~t uses  M~x  I/O perform~nce mode.  Mount the  EFS  le system on e~ch  EC2 inst~nce in the cluster.

 Correct ;;nswer: D
 D (48%)                                B (48%)                4%

 Question #395
 ;; comp~ny hosts ~ softw~re ~s ~ service (S~~S) solution on ;;WS. The solution h~s ~n ;;m~zon ;;PI G~tew~y ;;PI th~t serves ~n  HTTPS endpoint. The ;;PI uses ;;WS  L~mbd~ functions for compute. The  L~mbd~ functions store d~t~ in ~n ;;m~zon ;;uror~ Serverless v1 d~t~b~se. The comp~ny used the ;;WS Serverless ;;pplic~tion  Model (;;WS S;;M) to deploy the solution. The solution extends ~cross multiple ;;v~il~bility Zones ~nd h~s no dis~ster recovery (DR) pl~n. ;; solutions ~rchitect must design ~  DR str~tegy th~t c~n recover the solution in ~nother ;;WS  Region. The solution h~s ~n  RTO of 5 minutes ~nd ~n RPO of  1 minute. Wh~t should the solutions ~rchitect do to meet these requirements?
  ;;. Cre~te ~ re~d replic~ of the ;;uror~ Serverless v1 d~t~b~se in the t~rget  Region. Use ;;WS S;;M to cre~te ~ runbook to deploy the solution to the t~rget  Region.  Promote the re~d replic~ to prim~ry in c~se of dis~ster.
  B. Ch~nge the ;;uror~ Serverless v1 d~t~b~se to ~ st~nd~rd ;;uror~  MySQL glob~l d~t~b~se th~t extends ~cross the source  Region ~nd the t~rget  Region. Use ;;WS S;;M to cre~te ~ runbook to deploy the solution to the t~rget  Region.
  C. Cre~te ~n ;;uror~ Serverless v1  DB cluster th~t h~s multiple writer inst~nces in the t~rget  Region.  L~unch the solution in the t~rget  Region. Con gure the two  Region~l solutions to work in ~n ~ctive-p~ssive con gur~tion.
  D. Ch~nge the ;;uror~ Serverless v1 d~t~b~se to ~ st~nd~rd ;;uror~  MySQL glob~l d~t~b~se th~t extends ~cross the source  Region ~nd the t~rget  Region.  L~unch the solution in the t~rget  Region. Con gure the two  Region~l solutions to work in ~n ~ctive-p~ssive con gur~tion.

 Correct ;;nswer: B
 D (90%)                                    10%

 Question #396
 ;; comp~ny owns ~ ch~in of tr~vel ~gencies ~nd is running ~n ~pplic~tion in the ;;WS Cloud. Comp~ny employees use the ~pplic~tion to se~rch for inform~tion ~bout tr~vel destin~tions.  Destin~tion content is upd~ted four times e~ch ye~r. Two  xed ;;m~zon  EC2 inst~nces serve the ~pplic~tion. The comp~ny uses ~n ;;m~zon  Route 53 public hosted zone with ~ multiv~lue record of tr~vel.ex~mple.com th~t returns the  El~stic  IP ~ddresses for the  EC2 inst~nces. The ~pplic~tion uses ;;m~zon  Dyn~moDB ~s its prim~ry d~t~ store. The comp~ny uses ~ self-hosted  Redis inst~nce ~s ~ c~ching solution. During content upd~tes, the lo~d on the  EC2 inst~nces ~nd the c~ching solution incre~ses dr~stic~lly. This incre~sed lo~d h~s led to downtime on sever~l occ~sions. ;; solutions ~rchitect must upd~te the ~pplic~tion so th~t the ~pplic~tion is highly ~v~il~ble ~nd c~n h~ndle the lo~d th~t is gener~ted by the content upd~tes. Which solution will meet these requirements?
  ;;. Set up  Dyn~moDB ;;cceler~tor (D;;X) ~s in-memory c~che. Upd~te the ~pplic~tion to use  D;;X. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Set the ;;uto Sc~ling group ~s ~ t~rget for the ;;LB. Upd~te the  Route 53 record to use ~ simple routing policy th~t t~rgets the ;;LB's  DNS ~li~s. Con gure scheduled sc~ling for the  EC2 inst~nces before the content upd~tes.
  B. Set up ;;m~zon  El~stiC~che for  Redis. Upd~te the ~pplic~tion to use  El~stiC~che. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces. Cre~te ~n ;;m~zon CloudFront distribution, ~nd set the ;;uto Sc~ling group ~s ~n origin for the distribution. Upd~te the  Route 53 record to use ~ simple routing policy th~t t~rgets the CloudFront distribution’s  DNS ~li~s.  M~nu~lly sc~le up  EC2 inst~nces before the content upd~tes.
  C. Set up ;;m~zon  El~stiC~che for  Memc~ched. Upd~te the ~pplic~tion to use  El~stiC~che. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces. Cre~te ~n ;;pplic~tion  Lo~d  B~l~ncer (;;LB). Set the ;;uto Sc~ling group ~s ~ t~rget for the ;;LB. Upd~te the  Route 53 record to use ~ simple routing policy th~t t~rgets the ;;LB's  DNS ~li~s. Con gure scheduled sc~ling for the ~pplic~tion before the content upd~tes.
  D. Set up  Dyn~moDB ;;cceler~tor (D;;X) ~s in-memory c~che. Upd~te the ~pplic~tion to use  D;;X. Cre~te ~n ;;uto Sc~ling group for the  EC2 inst~nces. Cre~te ~n ;;m~zon CloudFront distribution, ~nd set the ;;uto Sc~ling group ~s ~n origin for the distribution. Upd~te the  Route 53 record to use ~ simple routing policy th~t t~rgets the CloudFront distribution's  DNS ~li~s.  M~nu~lly sc~le up  EC2 inst~nces before the content upd~tes.

 Correct ;;nswer: B
 ;; (95%)                                    5%

 Question #397
 ;; comp~ny needs to store ~nd process im~ge d~t~ th~t will be uplo~ded from mobile devices using ~ custom mobile ~pp. Us~ge pe~ks between 8 ;;M ~nd 5  PM on weekd~ys, with thous~nds of uplo~ds per minute. The ~pp is r~rely used ~t ~ny other time. ;; user is noti ed when im~ge processing is complete. Which combin~tion of ~ctions should ~ solutions ~rchitect t~ke to ensure im~ge processing c~n sc~le to h~ndle the lo~d? (Choose three.)
  ;;. Uplo~d  les from the mobile softw~re directly to ;;m~zon S3. Use S3 event noti c~tions to cre~te ~ mess~ge in ~n ;;m~zon  MQ queue.
  B. Uplo~d  les from the mobile softw~re directly to ;;m~zon S3. Use S3 event noti c~tions to cre~te ~ mess~ge in ~n ;;m~zon Simple Queue Service (;;m~zon SQS) st~nd~rd queue.
  C.  Invoke ~n ;;WS  L~mbd~ function to perform im~ge processing when ~ mess~ge is ~v~il~ble in the queue.
  D.  Invoke ~n S3  B~tch Oper~tions job to perform im~ge processing when ~ mess~ge is ~v~il~ble in the queue.
  E. Send ~ push noti c~tion to the mobile ~pp by using ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) when processing is complete.
  F. Send ~ push noti c~tion to the mobile ~pp by using ;;m~zon Simple  Em~il Service (;;m~zon SES) when processing is complete.

 Correct ;;nswer: ;;CD
 BCE (100%)

 Question #398
 ;; comp~ny is building ~n ~pplic~tion on ;;WS. The ~pplic~tion sends logs to ~n ;;m~zon OpenSe~rch Service cluster for ~n~lysis. ;;ll d~t~ must be stored within ~ VPC. Some of the comp~ny’s developers work from home. Other developers work from three different comp~ny o ce loc~tions. The developers need to ~ccess OpenSe~rch Service to ~n~lyze ~nd visu~lize logs directly from their loc~l development m~chines. Which solution will meet these requirements?
  ;;. Con gure ~nd set up ~n ;;WS Client VPN endpoint. ;;ssoci~te the Client VPN endpoint with ~ subnet in the VPC. Con gure ~ Client VPN self- service port~l.  Instruct the developers to connect by using the client for Client VPN.
  B. Cre~te ~ tr~nsit g~tew~y, ~nd connect it to the VPC. Cre~te ~n ;;WS Site-to-Site VPN. Cre~te ~n ~tt~chment to the tr~nsit g~tew~y.  Instruct the developers to connect by using ~n OpenVPN client.
  C. Cre~te ~ tr~nsit g~tew~y, ~nd connect it to the VPOrder ~n ;;WS  Direct Connect connection. Set up ~ public VIF on the  Direct Connect connection. ;;ssoci~te the public VIF with the tr~nsit g~tew~y.  Instruct the developers to connect to the  Direct Connect connection.
  D. Cre~te ~nd con gure ~ b~stion host in ~ public subnet of the VPC. Con gure the b~stion host security group to ~llow SSH ~ccess from the comp~ny CIDR r~nges.  Instruct the developers to connect by using SSH.

 Correct ;;nswer: D
 ;; (100%)

 Question #399
 ;; comp~ny w~nts to migr~te its website from ~n on-premises d~t~ center onto ;;WS. ;;t the s~me time, it w~nts to migr~te the website to ~ cont~inerized microservice-b~sed ~rchitecture to improve the ~v~il~bility ~nd cost e ciency. The comp~ny’s security policy st~tes th~t privileges ~nd network permissions must be con gured ~ccording to best pr~ctice, using le~st privilege. ;; solutions ~rchitect must cre~te ~ cont~inerized ~rchitecture th~t meets the security requirements ~nd h~s deployed the ~pplic~tion to ~n ;;m~zon  ECS cluster. Wh~t steps ~re required ~fter the deployment to meet the requirements? (Choose two.)
  ;;. Cre~te t~sks using the bridge network mode.
  B. Cre~te t~sks using the ~wsvpc network mode.
  C. ;;pply security groups to ;;m~zon  EC2 inst~nces, ~nd use  I;;M roles for  EC2 inst~nces to ~ccess other resources.
  D. ;;pply security groups to the t~sks, ~nd p~ss  I;;M credenti~ls into the cont~iner ~t l~unch time to ~ccess other resources.
  E. ;;pply security groups to the t~sks, ~nd use  I;;M roles for t~sks to ~ccess other resources.

 Correct ;;nswer: CD
 BE (100%)

 Question #400
 ;; comp~ny is running ~ serverless ~pplic~tion th~t consists of sever~l ;;WS  L~mbd~ functions ~nd ;;m~zon  Dyn~moDB t~bles. The comp~ny h~s cre~ted new function~lity th~t requires the  L~mbd~ functions to ~ccess ~n ;;m~zon  Neptune  DB cluster. The  Neptune  DB cluster is loc~ted in three subnets in ~ VPC. Which of the possible solutions will ~llow the  L~mbd~ functions to ~ccess the  Neptune  DB cluster ~nd  Dyn~moDB t~bles? (Choose two.)
  ;;. Cre~te three public subnets in the  Neptune VPC, ~nd route tr~ c through ~n internet g~tew~y.  Host the  L~mbd~ functions in the three new public subnets.
  B. Cre~te three priv~te subnets in the  Neptune VPC, ~nd route internet tr~ c through ~  N;;T g~tew~y.  Host the  L~mbd~ functions in the three new priv~te subnets.
  C.  Host the  L~mbd~ functions outside the VPUpd~te the  Neptune security group to ~llow ~ccess from the  IP r~nges of the  L~mbd~ functions.
  D.  Host the  L~mbd~ functions outside the VPC. Cre~te ~ VPC endpoint for the  Neptune d~t~b~se, ~nd h~ve the  L~mbd~ functions ~ccess Neptune over the VPC endpoint.
  E. Cre~te three priv~te subnets in the  Neptune VPC.  Host the  L~mbd~ functions in the three new isol~ted subnets. Cre~te ~ VPC endpoint for Dyn~moDB, ~nd route  Dyn~moDB tr~ c to the VPC endpoint.

 Correct ;;nswer: ;;E
 BE (91%)                                   9%

 Question #401
 ;; comp~ny w~nts to design ~ dis~ster recovery (DR) solution for ~n ~pplic~tion th~t runs in the comp~ny’s d~t~ center. The ~pplic~tion writes to ~n SMB  le sh~re ~nd cre~tes ~ copy on ~ second  le sh~re.  Both  le sh~res ~re in the d~t~ center. The ~pplic~tion uses two types of  les: met~d~t~  les ~nd im~ge  les. The comp~ny w~nts to store the copy on ;;WS. The comp~ny needs the ~bility to use SMB to ~ccess the d~t~ from either the d~t~ center or ;;WS if ~ dis~ster occurs. The copy of the d~t~ is r~rely ~ccessed but must be ~v~il~ble within 5 minutes.
  ;;.  Deploy ;;WS Outposts with ;;m~zon S3 stor~ge. Con gure ~ Windows ;;m~zon  EC2 inst~nce on Outposts ~s ~  le server.
  B.  Deploy ~n ;;m~zon  FSx  File G~tew~y. Con gure ~n ;;m~zon  FSx for Windows  File Server  Multi-;;Z  le system th~t uses SSD stor~ge.
  C.  Deploy ~n ;;m~zon S3  File G~tew~y. Con gure the S3  File G~tew~y to use ;;m~zon S3 St~nd~rd-Infrequent ;;ccess (S3 St~nd~rd-I;;) for the met~d~t~  les ~nd to use S3 Gl~cier  Deep ;;rchive for the im~ge  les.
  D.  Deploy ~n ;;m~zon S3  File G~tew~y. Con gure the S3  File G~tew~y to use ;;m~zon S3 St~nd~rd-Infrequent ;;ccess (S3 St~nd~rd-I;;) for the met~d~t~  les ~nd im~ge  les.

 Correct ;;nswer: D
 D (67%)                                  B (33%)

 Question #402
 ;; comp~ny is cre~ting ~ solution th~t c~n move 400 employees into ~ remote working environment in the event of ~n unexpected dis~ster. The user desktops h~ve ~ mix of Windows ~nd  Linux oper~ting systems.  Multiple types of softw~re, such ~s web browsers ~nd m~il clients, ~re inst~lled on e~ch desktop. ;; solutions ~rchitect needs to implement ~ solution th~t c~n be integr~ted with the comp~ny’s on-premises ;;ctive  Directory to ~llow employees to use their existing identity credenti~ls. The solution must provide multif~ctor ~uthentic~tion (MF;;) ~nd must replic~te the user experience from the existing desktops. Which solution will meet these requirements?
  ;;. Use ;;m~zon WorkSp~ces for the cloud desktop service. Set up ~ VPN connection to the on-premises network. Cre~te ~n ;;D Connector, ~nd connect to the on-premises ;;ctive  Directory. ;;ctiv~te  MF;; for ;;m~zon WorkSp~ces by using the ;;WS  M~n~gement Console.
  B. Use ;;m~zon ;;ppStre~m 2.0 ~s ~n ~pplic~tion stre~ming service. Con gure  Desktop View for the employees. Set up ~ VPN connection to the on-premises network. Set up ;;ctive  Directory  Feder~tion Services (;;D  FS) on premises. Connect the VPC network to ;;D  FS through the VPN connection.
  C. Use ;;m~zon WorkSp~ces for the cloud desktop service. Set up ~ VPN connection to the on-premises network. Cre~te ~n ;;D Connector, ~nd connect to the on-premises ;;ctive  Directory. Con gure ~  R;;DIUS server for  MF;;.
  D. Use ;;m~zon ;;ppStre~m 2.0 ~s ~n ~pplic~tion stre~ming service. Set up ;;ctive  Directory  Feder~tion Services on premises. Con gure  MF;; to gr~nt users ~ccess on ;;ppStre~m 2.0.

 Correct ;;nswer: C
 C (73%)                               ;; (20%)      7%

 Question #403
 ;; comp~ny h~s deployed ~n ;;m~zon Connect cont~ct center. Cont~ct center ~gents ~re reporting l~rge numbers of computer-gener~ted c~lls. The comp~ny is concerned ~bout the cost ~nd productivity effects of these c~lls. The comp~ny w~nts ~ solution th~t will ~llow ~gents to  ~g the c~ll ~s sp~m ~nd ~utom~tic~lly block the numbers from going to ~n ~gent in the future. Wh~t is the  MOST oper~tion~lly e cient solution to meet these requirements?
  ;;. Customize the Cont~ct Control  P~nel (CCP) by ~dding ~  ~g c~ll button th~t will invoke ~n ;;WS  L~mbd~ function th~t c~lls the Upd~teCont~ct;;ttributes ;;PI. Use ~n ;;m~zon  Dyn~moDB t~ble to store the sp~m numbers.  Modify the cont~ct  ows to look for the upd~ted ~ttribute ~nd to use ~  L~mbd~ function to re~d ~nd write to the  Dyn~moDB t~ble.
  B. Use ~ Cont~ct  Lens for ;;m~zon Connect rule th~t will look for sp~m c~lls. Use ~n ;;m~zon  Dyn~moDB t~ble to store the sp~m numbers. Modify the cont~ct  ows to look for the rule ~nd to invoke ~n ;;WS  L~mbd~ function to re~d ~nd write to the  Dyn~moDB t~ble.
  C. Use ~n ;;m~zon  Dyn~moDB t~ble to store the sp~m numbers. Cre~te ~ quick connect th~t the ~gents c~n tr~nsfer the sp~m c~ll to from the Cont~ct Control  P~nel (CCP).  Modify the quick connect cont~ct  ow to invoke ~n ;;WS  L~mbd~ function to write to the  Dyn~moDB t~ble.
  D.  Modify the initi~l cont~ct  ow to ~sk for c~ller input.  If the ~gent does not receive input, the ~gent should m~rk the c~ller ~s sp~m. Use ~n ;;m~zon  Dyn~moDB t~ble to store the sp~m numbers. Use ~n ;;WS  L~mbd~ function to re~d ~nd write to the  Dyn~moDB t~ble.

 Correct ;;nswer: B
 ;; (86%)                                   14%

 Question #404
 ;; comp~ny h~s mounted sensors to collect inform~tion ~bout environment~l p~r~meters such ~s humidity ~nd light throughout ~ll the comp~ny's f~ctories. The comp~ny needs to stre~m ~nd ~n~lyze the d~t~ in the ;;WS Cloud in re~l time.  If ~ny of the p~r~meters f~ll out of ~ccept~ble r~nges, the f~ctory oper~tions te~m must receive ~ noti c~tion immedi~tely. Which solution will meet these requirements?
  ;;. Stre~m the d~t~ to ~n ;;m~zon  Kinesis  D~t~  Firehose delivery stre~m. Use ;;WS Step  Functions to consume ~nd ~n~lyze the d~t~ in the Kinesis  D~t~  Firehose delivery stre~m. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to notify the oper~tions te~m.
  B. Stre~m the d~t~ to ~n ;;m~zon  M~n~ged Stre~ming for ;;p~che  K~fk~ (;;m~zon  MSK) cluster. Set up ~ trigger in ;;m~zon  MSK to invoke ~n ;;WS  F~rg~te t~sk to ~n~lyze the d~t~. Use ;;m~zon Simple  Em~il Service (;;m~zon SES) to notify the oper~tions te~m.
  C. Stre~m the d~t~ to ~n ;;m~zon  Kinesis d~t~ stre~m. Cre~te ~n ;;WS  L~mbd~ function to consume the  Kinesis d~t~ stre~m ~nd to ~n~lyze the d~t~. Use ;;m~zon Simple  Noti c~tion Service (;;m~zon SNS) to notify the oper~tions te~m.
  D. Stre~m the d~t~ to ~n ;;m~zon  Kinesis  D~t~ ;;n~lytics ~pplic~tion. Use ~n ~utom~tic~lly sc~led ~nd cont~inerized service in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS) to consume ~nd ~n~lyze the d~t~. Use ;;m~zon Simple  Em~il Service (;;m~zon SES) to notify the oper~tions te~m.

 Correct ;;nswer: B
 C (100%)

 Question #405
 ;; comp~ny is prep~ring to deploy ~n ;;m~zon  El~stic  Kubernetes Service (;;m~zon  EKS) cluster for ~ worklo~d. The comp~ny expects the cluster to support ~n unpredict~ble number of st~teless pods.  M~ny of the pods will be cre~ted during ~ short time period ~s the worklo~d ~utom~tic~lly sc~les the number of replic~s th~t the worklo~d uses. Which solution will  M;;XIMIZE node resilience?
  ;;. Use ~ sep~r~te l~unch templ~te to deploy the  EKS control pl~ne into ~ second cluster th~t is sep~r~te from the worklo~d node groups.
  B. Upd~te the worklo~d node groups. Use ~ sm~ller number of node groups ~nd l~rger inst~nces in the node groups.
  C. Con gure the  Kubernetes Cluster ;;utosc~ler to ensure th~t the compute c~p~city of the worklo~d node groups st~ys underprovisioned.
  D. Con gure the worklo~d to use topology spre~d constr~ints th~t ~re b~sed on ;;v~il~bility Zone.

 Correct ;;nswer: D
 D (89%)                                    11%

 Question #406
 ;; comp~ny needs to implement ~ dis~ster recovery (DR) pl~n for ~ web ~pplic~tion. The ~pplic~tion runs in ~ single ;;WS  Region. The ~pplic~tion uses microservices th~t run in cont~iners. The cont~iners ~re hosted on ;;WS  F~rg~te in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS). The ~pplic~tion h~s ~n ;;m~zon  RDS for  MySQL  DB inst~nce ~s its d~t~ l~yer ~nd uses ;;m~zon  Route 53 for  DNS resolution. ;;n ;;m~zon CloudW~tch ~l~rm invokes ~n ;;m~zon  EventBridge rule if the ~pplic~tion experiences ~ f~ilure. ;; solutions ~rchitect must design ~  DR solution to provide ~pplic~tion recovery to ~ sep~r~te  Region. The solution must minimize the time th~t is necess~ry to recover from ~ f~ilure. Which solution will meet these requirements?
  ;;. Setup ~ second  ECS cluster ~nd  ECS service on  F~rg~te in the sep~r~te  Region. Cre~te ~n ;;WS  L~mbd~ function to perform the following ~ctions: t~ke ~ sn~pshot of the  RDS  DB inst~nce, copy the sn~pshot to the sep~r~te  Region, cre~te ~ new  RDS  DB inst~nce from the sn~pshot, ~nd upd~te  Route 53 to route tr~ c to the second  ECS cluster. Upd~te the  EventBridge rule to ~dd ~ t~rget th~t will invoke the  L~mbd~ function.
  B. Cre~te ~n ;;WS  L~mbd~ function th~t cre~tes ~ second  ECS cluster ~nd  ECS service in the sep~r~te  Region. Con gure the  L~mbd~ function to perform the following ~ctions: t~ke ~ sn~pshot of the  RDS  DB inst~nce, copy the sn~pshot to the sep~r~te  Region, cre~te ~ new  RDS  DB inst~nce from the sn~pshot, ~nd upd~te  Route 53 to route tr~ c to the second  ECS cluster. Upd~te the  EventBridge rule to ~dd ~ t~rget th~t will invoke the  L~mbd~ function.
  C. Setup ~ second  ECS cluster ~nd  ECS service on  F~rg~te in the sep~r~te  Region. Cre~te ~ cross-Region re~d replic~ of the  RDS  DB inst~nce in the sep~r~te  Region. Cre~te ~n ;;WS  L~mbd~ function to promote the re~d replic~ to the prim~ry d~t~b~se. Con gure the  L~mbd~ function to upd~te  Route 53 to route tr~ c to the second  ECS cluster. Upd~te the  EventBridge rule to ~dd ~ t~rget th~t will invoke the  L~mbd~ function.
  D. Setup ~ second  ECS cluster ~nd  ECS service on  F~rg~te in the sep~r~te  Region. T~ke ~ sn~pshot of the  RDS  DB inst~nce. Convert the sn~pshot to ~n ;;m~zon  Dyn~moDB glob~l t~ble. Cre~te ~n ;;WS  L~mbd~ function to upd~te  Route 53 to route tr~ c to the second  ECS cluster. Upd~te the  EventBridge rule to ~dd ~ t~rget th~t will invoke the  L~mbd~ function.

 Correct ;;nswer: ;;
 C (100%)

 Question #407
 ;; comp~ny h~s ;;WS ~ccounts th~t ~re in ~n org~niz~tion in ;;WS Org~niz~tions. The comp~ny w~nts to tr~ck ;;m~zon  EC2 us~ge ~s ~ metric. The comp~ny’s ~rchitecture te~m must receive ~ d~ily ~lert if the  EC2 us~ge is more th~n  10% higher the ~ver~ge  EC2 us~ge from the l~st 30 d~ys. Which solution will meet these requirements?
  ;;. Con gure ;;WS  Budgets in the org~niz~tion's m~n~gement ~ccount. Specify ~ us~ge type of  EC2 running hours. Specify ~ d~ily period. Set the budget ~mount to be  10% more th~n the reported ~ver~ge us~ge for the l~st 30 d~ys from ;;WS Cost  Explorer. Con gure ~n ~lert to notify the ~rchitecture te~m if the us~ge threshold is met
  B. Con gure ;;WS Cost ;;nom~ly  Detection in the org~niz~tion's m~n~gement ~ccount. Con gure ~ monitor type of ;;WS Service. ;;pply ~  lter of ;;m~zon  EC2. Con gure ~n ~lert subscription to notify the ~rchitecture te~m if the us~ge is  10% more th~n the ~ver~ge us~ge for the l~st 30 d~ys.
  C.  En~ble ;;WS Trusted ;;dvisor in the org~niz~tion's m~n~gement ~ccount. Con gure ~ cost optimiz~tion ~dvisory ~lert to notify the ~rchitecture te~m if the  EC2 us~ge is  10% more th~n the reported ~ver~ge us~ge for the l~st 30 d~ys.
  D. Con gure ;;m~zon  Detective in the org~niz~tion's m~n~gement ~ccount. Con gure ~n  EC2 us~ge ~nom~ly ~lert to notify the ~rchitecture te~m if  Detective identi es ~ us~ge ~nom~ly of more th~n  10%.

 Correct ;;nswer: C
 ;; (70%)                                  B (30%)

 Question #408
 ;;n e-commerce comp~ny is rev~mping its  IT infr~structure ~nd is pl~nning to use ;;WS services. The comp~ny’s CIO h~s ~sked ~ solutions ~rchitect to design ~ simple, highly ~v~il~ble, ~nd loosely coupled order processing ~pplic~tion. The ~pplic~tion is responsible for receiving ~nd processing orders before storing them in ~n ;;m~zon  Dyn~moDB t~ble. The ~pplic~tion h~s ~ spor~dic tr~ c p~ttern ~nd should be ~ble to sc~le during m~rketing c~mp~igns to process the orders with minim~l del~ys. Which of the following is the  MOST reli~ble ~ppro~ch to meet the requirements?
  ;;.  Receive the orders in ~n ;;m~zon  EC2-hosted d~t~b~se ~nd use  EC2 inst~nces to process them.
  B.  Receive the orders in ~n ;;m~zon SQS queue ~nd invoke ~n ;;WS  L~mbd~ function to process them.
  C.  Receive the orders using the ;;WS Step  Functions progr~m ~nd l~unch ~n ;;m~zon  ECS cont~iner to process them.
  D.  Receive the orders in ;;m~zon  Kinesis  D~t~ Stre~ms ~nd use ;;m~zon  EC2 inst~nces to process them.

 Correct ;;nswer: C
 B (78%)                                  C (22%)

 Question #409
 ;; comp~ny is deploying ;;WS  L~mbd~ functions th~t ~ccess ~n ;;m~zon  RDS for  PostgreSQL d~t~b~se. The comp~ny needs to l~unch the  L~mbd~ functions in ~ Q;; environment ~nd in ~ production environment. The comp~ny must not expose credenti~ls within ~pplic~tion code ~nd must rot~te p~sswords ~utom~tic~lly. Which solution will meet these requirements?
  ;;. Store the d~t~b~se credenti~ls for both environments in ;;WS Systems  M~n~ger  P~r~meter Store.  Encrypt the credenti~ls by using ~n ;;WS Key  M~n~gement Service (;;WS  KMS) key. Within the ~pplic~tion code of the  L~mbd~ functions, pull the credenti~ls from the  P~r~meter Store p~r~meter by using the ;;WS SDK for  Python (Boto3). ;;dd ~ role to the  L~mbd~ functions to provide ~ccess to the  P~r~meter Store p~r~meter.
  B. Store the d~t~b~se credenti~ls for both environments in ;;WS Secrets  M~n~ger with distinct key entry for the Q;; environment ~nd the production environment. Turn on rot~tion.  Provide ~ reference to the Secrets  M~n~ger key ~s ~n environment v~ri~ble for the  L~mbd~ functions.
  C. Store the d~t~b~se credenti~ls for both environments in ;;WS  Key  M~n~gement Service (;;WS  KMS). Turn on rot~tion.  Provide ~ reference to the credenti~ls th~t ~re stored in ;;WS  KMS ~s ~n environment v~ri~ble for the  L~mbd~ functions.
  D. Cre~te sep~r~te S3 buckets for the Q;; environment ~nd the production environment. Turn on server-side encryption with ;;WS  KMS keys (SSE-KMS) for the S3 buckets. Use ~n object n~ming p~ttern th~t gives e~ch  L~mbd~ function’s ~pplic~tion code the ~bility to pull the correct credenti~ls for the function's corresponding environment. Gr~nt e~ch  L~mbd~ function's execution role ~ccess to ;;m~zon S3.

 Correct ;;nswer: ;;
 B (100%)

 Question #410
 ;; comp~ny is using ;;WS Control Tower to m~n~ge ;;WS ~ccounts in ~n org~niz~tion in ;;WS Org~niz~tions. The comp~ny h~s ~n OU th~t cont~ins ~ccounts. The comp~ny must prevent ~ny new or existing ;;m~zon  EC2 inst~nces in the OU's ~ccounts from g~ining ~ public  IP ~ddress. Which solution will meet these requirements?
  ;;. Con gure ~ll inst~nces in e~ch ~ccount in the OU to use ;;WS Systems  M~n~ger. Use ~ Systems  M~n~ger ;;utom~tion runbook to prevent public  IP ~ddresses from being ~tt~ched to the inst~nces.
  B.  Implement the ;;WS Control Tower pro~ctive control to check whether inst~nces in the OU's ~ccounts h~ve ~ public  IP ~ddress. Set the ;;ssoci~tePublicIp;;ddress property to  F~lse. ;;tt~ch the pro~ctive control to the OU.
  C. Cre~te ~n SCP th~t prevents the l~unch of inst~nces th~t h~ve ~ public  IP ~ddress. ;;ddition~lly, con gure the SCP to prevent the ~tt~chment of ~ public  IP ~ddress to existing inst~nces. ;;tt~ch the SCP to the OU.
  D. Cre~te ~n ;;WS Con g custom rule th~t detects inst~nces th~t h~ve ~ public  IP ~ddress. Con gure ~ remedi~tion ~ction th~t uses ~n ;;WS L~mbd~ function to det~ch the public  IP ~ddresses from the inst~nces.

 Correct ;;nswer: D
 C (100%)

 Question #411
 ;; comp~ny is deploying ~ third-p~rty web ~pplic~tion on ;;WS. The ~pplic~tion is p~ck~ged ~s ~  Docker im~ge. The comp~ny h~s deployed the Docker im~ge ~s ~n ;;WS  F~rg~te service in ;;m~zon  El~stic Cont~iner Service (;;m~zon  ECS). ;;n ;;pplic~tion  Lo~d  B~l~ncer (;;LB) directs tr~ c to the ~pplic~tion. The comp~ny needs to give only ~ speci c list of users the ~bility to ~ccess the ~pplic~tion from the internet. The comp~ny c~nnot ch~nge the ~pplic~tion ~nd c~nnot integr~te the ~pplic~tion with ~n identity provider. ;;ll users must be ~uthentic~ted through multi-f~ctor ~uthentic~tion (MF;;). Which solution will meet these requirements?
  ;;. Cre~te ~ user pool in ;;m~zon Cognito. Con gure the pool for the ~pplic~tion.  Popul~te the pool with the required users. Con gure the pool to require  MFCon gure ~ listener rule on the ;;LB to require ~uthentic~tion through the ;;m~zon Cognito hosted UI.
  B. Con gure the users in ;;WS  Identity ~nd ;;ccess  M~n~gement (I;;M). ;;tt~ch ~ resource policy to the  F~rg~te service to require users to use MF;;. Con gure ~ listener rule on the ;;LB to require ~uthentic~tion through  I;;M.
  C. Con gure the users in ;;WS  Identity ~nd ;;ccess  M~n~gement (I;;M).  En~ble ;;WS  I;;M  Identity Center (;;WS Single Sign-On). Con gure resource protection for the ;;LB. Cre~te ~ resource protection rule to require users to use  MF;;.
  D. Cre~te ~ user pool in ;;WS ;;mplify. Con gure the pool for the ~pplic~tion.  Popul~te the pool with the required users. Con gure the pool to require  MF;;. Con gure ~ listener rule on the ;;LB to require ~uthentic~tion through the ;;mplify hosted UI.

 Correct ;;nswer: ;;
 ;; (75%)                                  U (25%)
