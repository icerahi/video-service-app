# video-service-app
Model Architecture planning

<i>Membership
>>slug

>>type(free,pro,enterprise)

>>price

>>stipe plan id

<i>UserMembership
>> user (foreignkey to default)

>>stripe customer id

>> membership type  (foreignkey to Membership)

<i> Subcription

>> user membership

>>stripe subscription id  (foreignkey to UserMembership)

>> active

<i> Course
 
 >> slug
 
 >>title
 
 >>description
 
 >> allowed memberships (foreignkey to membership)
 
 <li> Lession
 
 >> slug
 
 >>title
 
 >>Course  (foreignkey to Course)
 
 >>position
 
 >>video
 
 >>thumbnail