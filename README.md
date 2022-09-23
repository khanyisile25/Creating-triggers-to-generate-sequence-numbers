# Creating-triggers-to-generate-sequence-numbers

Technology used my sql XAAMP
created triggers in database so that it generates the sequence numbers also the system date 

#first create a table in database
#id table
#users table
#create triggers
#code for triggers
BEGIN
    INSERT INTO id_value_tbl VALUES(NULL);
    SET NEW.rec_id = CONCAT("STC_", SYSDATE(),LPAD(LAST_INSERT_ID(), 3, "0"));
    END
