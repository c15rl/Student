# Student
CS3 assignment (Dalton)
import java.io.File;
import java.util.HashSet;
import java.util.List;
import java.util.Arrays;
import java.util.ArrayList;
import java.util.Set;

public class Student {

	String stats;
	String first;
	String middle;
	String last;
	String gender;
	String grade_entered;
	String grade_current;
	String grad;
	String day;
	String month;
	String year;
	String house;
	List<String> all_info;

	/**
	 * sorts all of the info about an individual student
	 * @param line	one entry from data in database of students
	 */
	public Student(String line){
		this.stats=line + "\n";
		String[] holder = line.split(",");
		this.first = holder[0];
		this.middle = holder[1];
		this.last = holder[2];
		this.gender = holder[3];
		this.grade_entered = holder[4];
		this.grade_current = holder[5];
		this.grad = holder[6];
		this.day = holder[7];
		this.month = holder[8];
		this.year = holder[9];
		this.house = holder[10];
		this.all_info = Arrays.asList(holder);
		// split information here
		// put correct parts of split in correct instance variable, e.g., this.stats=line

	}

	public String toString() {
		return this.stats;
	}


}


