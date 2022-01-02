# python_flask_api

GET /doctors/ -> List all doctors
GET /doctors/:id -> Get a specific doctor
GET /doctors/:id/appointments -> List all appointments for a doctor
GET /doctors/:id/appointments?date=xyz -> List all appointments for a doctor with specific date
POST /doctors/:id/appointments/ -> Add a new appointment
Body {
    id: number,
    firstName: string,
    lastName: string,
    date: string,
    time: string,
    kind: 'New Patient' | 'Follow-up'
    #(should be new or follow up)
}
DEL /doctors/:id/appointments/:appointmentId -> Delete a specific appointment for a doctor
