# XenonStackTechincalTask_cdac
Details about Project:
1.Project Name:-Basic employee Regestration,Login form. 
 FrontEND:- Html,Thymleaf,Bootstrap used.
 BackEND:- Java-SpringBoot2.7 used.
 Database:- MySQL used.
****************************************************************************************************
2.Application flow :-
     Browser<->userRegistrationController<->UserService<->UserRepository<->MySQL
       <1>            <2>                       <3>              <4>          <5>
i> When user hit Browser,the httpRequest will 1st come to the <UserRegistrationController> 
   This is basically Spring MVC controller,which will handle httpRequest like GET,POST.
ii> and request will move from <UserService> to <UserRepository>and it finally hit to the database.
iii> so,userRepo will retrive data from MySQL goes to ->UserRepository->userRegistrationController.
    and finally,userRegistrationController will return a view,i.e.Thymleaf-Html-Template to Browser 
    for Rendering.
******************************************************************************************************   
3.Application Architecture:-
  3 Layer Architecture used-> UserRegistrationController(SpringMVC used),UserService(Service-Layer),UserRepository(DAO-Layer). 
  *UserRegistrationController:->SpringMVC used which handle httpRequest
  *UserServiceLayer          :->We keep our business Logic,Transaction related info here.
  *UserRepository            :->We are going to develop a JPA repositories using Spring-dataJPA to interact with Database. 
                                using Spring-dataJPA to basically reduce BoilerPlate code that is required for
                                developing code operations for Database.
******************************************************************************************************* 
 4. A project screenshot of output step by step are also added.
  
